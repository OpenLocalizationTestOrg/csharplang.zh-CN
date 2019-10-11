---
title: 可在 Azure Active Directory B2C 中使用的应用程序类型
description: 了解可与 Azure Active Directory B2C 一起使用的应用程序类型。
services: active-directory-b2c
author: mmacy
manager: celestedg
ms.service: active-directory
ms.workload: identity
ms.topic: conceptual
ms.date: 07/24/2019
ms.author: marsma
ms.subservice: B2C
ms.openlocfilehash: ed75116801a0a8f7af23bf879383cc6b4d7a59ea
ms.sourcegitcommit: 036e4e16d0416fabfc6b4439fdd726b68e3f7373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "6609445"
---
# <a name="application-types-that-can-be-used-in-active-directory-b2c"></a>可在 Active Directory B2C 中使用的应用程序类型

Azure Active Directory B2C （Azure AD B2C）支持多种新式应用程序体系结构的身份验证。 所有这些都基于行业标准协议[OAuth 2.0](active-directory-b2c-reference-protocols.md)或[OpenID connect](active-directory-b2c-reference-protocols.md)。 本文介绍了你可以构建的应用程序类型，这些类型与你喜欢的语言或平台无关。 它还可帮助你在开始构建应用程序之前了解高级方案。

使用 Azure AD B2C 的每个应用程序都必须使用[Azure 门户](https://portal.azure.com/)在[Azure AD B2C 租户](active-directory-b2c-get-started.md)中进行注册。 应用程序注册过程将收集并分配值，例如：

* 唯一标识应用程序的**应用程序 ID** 。
* 可用于将响应定向回应用程序的**答复 URL** 。

发送给 Azure AD B2C 的每个请求都指定了一个**用户流**（内置策略）或控制 Azure AD B2C 行为的**自定义策略**。 这两种策略类型都使你能够创建一组高度可自定义的用户体验。

每个应用程序的交互遵循类似的高级模式：

1. 应用程序会将用户定向到 v2.0 终结点，以执行[策略](active-directory-b2c-reference-policies.md)。
2. 用户根据策略定义完成策略。
3. 应用程序从 v2.0 终结点接收安全令牌。
4. 应用程序使用安全令牌来访问受保护的信息或受保护的资源。
5. 资源服务器将验证安全令牌，以验证是否可以授予访问权限。
6. 应用程序定期刷新安全令牌。

根据要生成的应用程序类型，这些步骤可能稍有不同。

## <a name="web-applications"></a>Web 应用程序

对于在服务器上托管并通过浏览器访问的 web 应用程序（包括 .NET、PHP、Java、Ruby、Python 和 node.js），Azure AD B2C 支持使用[OpenID connect](active-directory-b2c-reference-protocols.md)实现所有用户体验。 在 OpenID Connect Azure AD B2C 实现中，web 应用程序通过向 Azure AD 发出身份验证请求来启动用户体验。 请求的结果是 @no__t 0。 此安全令牌表示用户的标识。 它还以声明形式提供有关用户的信息：

```json
// Partial raw id_token
eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6ImtyaU1QZG1Cd...

// Partial content of a decoded id_token
{
    "name": "John Smith",
    "email": "john.smith@gmail.com",
    "oid": "d9674823-dffc-4e3f-a6eb-62fe4bd48a58"
    ...
}
```

详细了解[Azure AD B2C 令牌引用](active-directory-b2c-reference-tokens.md)中可用于应用程序的令牌类型和声明。

在 web 应用程序中，每次执行[策略](active-directory-b2c-reference-policies.md)都要执行以下高级步骤：

1. 用户浏览到 web 应用程序。
2. Web 应用程序将用户重定向到 Azure AD B2C，以指示要执行的策略。
3. 用户完成策略。
4. Azure AD B2C 在浏览器中返回 @no__t 0。
5. @No__t 将发布到重定向 URI。
6. 验证 `id_token` 并设置会话 cookie。
7. 将向用户返回一个安全页。

使用从 Azure AD 接收的公共签名密钥验证 `id_token` 足以验证用户的身份。 此过程还会设置会话 cookie，可用于在后续页面请求中标识用户。

若要查看此方案的运行情况，请尝试在 "入门"[部分](active-directory-b2c-overview.md)中提供 web 应用程序登录代码示例之一。

除了便于简单登录，web 服务器应用程序还可能需要访问后端 web 服务。 在这种情况下，web 应用程序可以执行略有不同的[OpenID connect 流](active-directory-b2c-reference-oidc.md)，并使用授权代码和刷新令牌来获取令牌。 下面的[Web api 部分](#web-apis)描述了此方案。

## <a name="web-apis"></a>Web Api

你可以使用 Azure AD B2C 来保护 web 服务，例如应用程序的 RESTful web API。 Web Api 可以使用 OAuth 2.0 通过使用令牌对传入的 HTTP 请求进行身份验证来保护其数据。 Web API 的调用方在 HTTP 请求的授权标头中追加一个标记：

```
GET /api/items HTTP/1.1
Host: www.mywebapi.com
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6...
Accept: application/json
...
```

然后，web API 可以使用令牌来验证 API 调用方的标识，并从令牌中编码的声明提取有关调用方的信息。 详细了解[Azure AD B2C 令牌参考](active-directory-b2c-reference-tokens.md)中的应用可用的令牌和声明类型。

Web API 可以从许多类型的客户端（包括 web 应用程序、桌面和移动应用程序、单页应用程序、服务器端守护程序以及其他 web Api）接收令牌。 下面是用于调用 web API 的 web 应用程序的完整流示例：

1. Web 应用程序执行策略，用户完成用户体验。
2. Azure AD B2C 返回（OpenID Connect） `id_token`，并向浏览器返回一个授权代码。
3. 浏览器将 @no__t 0 和授权代码发送到重定向 URI。
4. Web 服务器验证 `id_token` 并设置会话 cookie。
5. Web 服务器通过向其提供授权代码、应用程序客户端 ID 和客户端凭据来请求 @no__t Azure AD B2C。
6. 将 `access_token` 和 `refresh_token` 返回到 web 服务器。
7. 使用授权标头中的 `access_token` 调用 web API。
8. Web API 将验证令牌。
9. 安全数据将返回到 web 应用程序。

若要详细了解授权代码、刷新令牌和获取令牌的步骤，请参阅[OAuth 2.0 协议](active-directory-b2c-reference-oauth-code.md)。

若要了解如何使用 Azure AD B2C 保护 web API，请参阅[入门部分](active-directory-b2c-overview.md)中的 web api 教程。

## <a name="mobile-and-native-applications"></a>移动和本机应用程序

安装在设备上的应用程序（如移动和桌面应用程序）通常需要代表用户访问后端服务或 web Api。 你可以通过使用 Azure AD B2C 和[OAuth 2.0 授权代码流](active-directory-b2c-reference-oauth-code.md)，将自定义的标识管理体验添加到本机应用程序并安全调用后端服务。

在此流中，应用程序执行[策略](active-directory-b2c-reference-policies.md)，并在用户完成策略后从 Azure AD 接收 @no__t。 @No__t-0 表示应用程序代表当前登录用户调用后端服务的权限。 然后，应用程序可以在后台为 @no__t 和 @no__t 交换 `authorization_code`。  应用程序可以使用 `access_token` 向 HTTP 请求中的后端 web API 进行身份验证。 它还可以使用 `refresh_token` 在旧的 @no__t 过期时获取新的。

## <a name="current-limitations"></a>当前限制

### <a name="unsupported-application-types"></a>不受支持的应用程序类型

#### <a name="daemonsserver-side-applications"></a>守护程序/服务器端应用程序

包含长时间运行的进程或在没有用户的情况下运行的应用程序还需要通过某种方式来访问受保护的资源（如 web Api）。 这些应用程序可以通过使用应用程序的标识（而不是用户的委派标识）和 OAuth 2.0 客户端凭据流来对令牌进行身份验证和获取令牌。 客户端凭据流不同于代表流，而且不应用于服务器到服务器的身份验证流。

尽管 Azure AD B2C 当前不支持客户端凭据流，但你可以使用 Azure AD 设置客户端凭据流。 Azure AD B2C 租户与 Azure AD 企业租户共享某些功能。  使用 Azure AD B2C 租户的 Azure AD 功能支持客户端凭据流。

若要设置客户端凭据流，请参阅[Azure Active Directory v2.0 和 OAuth 2.0 客户端凭据流](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds)。 身份验证成功后，将收到已设置格式的令牌，以便 Azure AD 如[Azure AD 令牌参考](https://docs.microsoft.com/azure/active-directory/develop/active-directory-token-and-claims)中所述。

#### <a name="web-api-chains-on-behalf-of-flow"></a>Web API 链（代理流）

许多体系结构包含需要调用另一个下游 web API 的 web API，这两者都受 Azure AD B2C 保护。 此方案常见于具有 Web API 后端的本机客户端，并调用 Microsoft online 服务（例如 Azure AD 图形 API）。

可以通过使用 OAuth 2.0 JWT 持有者凭据授权（也称为代理流）来支持这种链接的 web API 方案。  但 Azure AD B2C 中当前未实现代理流。

### <a name="faulted-apps"></a>出错的应用

不要通过以下方式编辑 Azure AD B2C 应用程序：

- 在其他应用程序管理门户上，如[应用程序注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)。
- 使用图形 API 或 PowerShell。

如果在 Azure 门户之外编辑 Azure AD B2C 应用程序，则该应用程序将成为出错的应用程序，并且不能再与 Azure AD B2C 一起使用。 删除并重新创建应用程序。

若要删除应用程序，请在[应用程序注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中，并删除该应用程序。 为了使应用程序可见，你需要是应用程序的所有者（而不只是租户的管理员）。

## <a name="next-steps"></a>后续步骤

了解有关[Azure Active Directory B2C 中的用户流](active-directory-b2c-reference-policies.md)提供的内置策略的详细信息。
