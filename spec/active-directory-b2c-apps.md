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
# <a name="application-types-that-can-be-used-in-active-directory-b2c"></a><span data-ttu-id="964e3-103">可在 Active Directory B2C 中使用的应用程序类型</span><span class="sxs-lookup"><span data-stu-id="964e3-103">Application types that can be used in Active Directory B2C</span></span>

<span data-ttu-id="964e3-104">Azure Active Directory B2C （Azure AD B2C）支持多种新式应用程序体系结构的身份验证。</span><span class="sxs-lookup"><span data-stu-id="964e3-104">Azure Active Directory B2C (Azure AD B2C) supports authentication for a variety of modern application architectures.</span></span> <span data-ttu-id="964e3-105">所有这些都基于行业标准协议[OAuth 2.0](active-directory-b2c-reference-protocols.md)或[OpenID connect](active-directory-b2c-reference-protocols.md)。</span><span class="sxs-lookup"><span data-stu-id="964e3-105">All of them are based on the industry standard protocols [OAuth 2.0](active-directory-b2c-reference-protocols.md) or [OpenID Connect](active-directory-b2c-reference-protocols.md).</span></span> <span data-ttu-id="964e3-106">本文介绍了你可以构建的应用程序类型，这些类型与你喜欢的语言或平台无关。</span><span class="sxs-lookup"><span data-stu-id="964e3-106">This article describes the types of applications that you can build, independent of the language or platform you prefer.</span></span> <span data-ttu-id="964e3-107">它还可帮助你在开始构建应用程序之前了解高级方案。</span><span class="sxs-lookup"><span data-stu-id="964e3-107">It also helps you understand the high-level scenarios before you start building applications.</span></span>

<span data-ttu-id="964e3-108">使用 Azure AD B2C 的每个应用程序都必须使用[Azure 门户](https://portal.azure.com/)在[Azure AD B2C 租户](active-directory-b2c-get-started.md)中进行注册。</span><span class="sxs-lookup"><span data-stu-id="964e3-108">Every application that uses Azure AD B2C must be registered in your [Azure AD B2C tenant](active-directory-b2c-get-started.md) by using the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="964e3-109">应用程序注册过程将收集并分配值，例如：</span><span class="sxs-lookup"><span data-stu-id="964e3-109">The application registration process collects and assigns values, such as:</span></span>

* <span data-ttu-id="964e3-110">唯一标识应用程序的**应用程序 ID** 。</span><span class="sxs-lookup"><span data-stu-id="964e3-110">An **Application ID** that uniquely identifies your application.</span></span>
* <span data-ttu-id="964e3-111">可用于将响应定向回应用程序的**答复 URL** 。</span><span class="sxs-lookup"><span data-stu-id="964e3-111">A **Reply URL** that can be used to direct responses back to your application.</span></span>

<span data-ttu-id="964e3-112">发送给 Azure AD B2C 的每个请求都指定了一个**用户流**（内置策略）或控制 Azure AD B2C 行为的**自定义策略**。</span><span class="sxs-lookup"><span data-stu-id="964e3-112">Each request that is sent to Azure AD B2C specifies a **user flow** (a built-in policy) or a **custom policy** that controls the behavior of Azure AD B2C.</span></span> <span data-ttu-id="964e3-113">这两种策略类型都使你能够创建一组高度可自定义的用户体验。</span><span class="sxs-lookup"><span data-stu-id="964e3-113">Both policy types enable you to create a highly customizable set of user experiences.</span></span>

<span data-ttu-id="964e3-114">每个应用程序的交互遵循类似的高级模式：</span><span class="sxs-lookup"><span data-stu-id="964e3-114">The interaction of every application follows a similar high-level pattern:</span></span>

1. <span data-ttu-id="964e3-115">应用程序会将用户定向到 v2.0 终结点，以执行[策略](active-directory-b2c-reference-policies.md)。</span><span class="sxs-lookup"><span data-stu-id="964e3-115">The application directs the user to the v2.0 endpoint to execute a [policy](active-directory-b2c-reference-policies.md).</span></span>
2. <span data-ttu-id="964e3-116">用户根据策略定义完成策略。</span><span class="sxs-lookup"><span data-stu-id="964e3-116">The user completes the policy according to the policy definition.</span></span>
3. <span data-ttu-id="964e3-117">应用程序从 v2.0 终结点接收安全令牌。</span><span class="sxs-lookup"><span data-stu-id="964e3-117">The application receives a security token from the v2.0 endpoint.</span></span>
4. <span data-ttu-id="964e3-118">应用程序使用安全令牌来访问受保护的信息或受保护的资源。</span><span class="sxs-lookup"><span data-stu-id="964e3-118">The application uses the security token to access protected information or a protected resource.</span></span>
5. <span data-ttu-id="964e3-119">资源服务器将验证安全令牌，以验证是否可以授予访问权限。</span><span class="sxs-lookup"><span data-stu-id="964e3-119">The resource server validates the security token to verify that access can be granted.</span></span>
6. <span data-ttu-id="964e3-120">应用程序定期刷新安全令牌。</span><span class="sxs-lookup"><span data-stu-id="964e3-120">The application periodically refreshes the security token.</span></span>

<span data-ttu-id="964e3-121">根据要生成的应用程序类型，这些步骤可能稍有不同。</span><span class="sxs-lookup"><span data-stu-id="964e3-121">These steps can differ slightly based on the type of application you're building.</span></span>

## <a name="web-applications"></a><span data-ttu-id="964e3-122">Web 应用程序</span><span class="sxs-lookup"><span data-stu-id="964e3-122">Web applications</span></span>

<span data-ttu-id="964e3-123">对于在服务器上托管并通过浏览器访问的 web 应用程序（包括 .NET、PHP、Java、Ruby、Python 和 node.js），Azure AD B2C 支持使用[OpenID connect](active-directory-b2c-reference-protocols.md)实现所有用户体验。</span><span class="sxs-lookup"><span data-stu-id="964e3-123">For web applications (including .NET, PHP, Java, Ruby, Python, and Node.js) that are hosted on a server and accessed through a browser, Azure AD B2C supports [OpenID Connect](active-directory-b2c-reference-protocols.md) for all user experiences.</span></span> <span data-ttu-id="964e3-124">在 OpenID Connect Azure AD B2C 实现中，web 应用程序通过向 Azure AD 发出身份验证请求来启动用户体验。</span><span class="sxs-lookup"><span data-stu-id="964e3-124">In the Azure AD B2C implementation of OpenID Connect, your web application initiates user experiences by issuing authentication requests to Azure AD.</span></span> <span data-ttu-id="964e3-125">请求的结果是 @no__t 0。</span><span class="sxs-lookup"><span data-stu-id="964e3-125">The result of the request is an `id_token`.</span></span> <span data-ttu-id="964e3-126">此安全令牌表示用户的标识。</span><span class="sxs-lookup"><span data-stu-id="964e3-126">This security token represents the user's identity.</span></span> <span data-ttu-id="964e3-127">它还以声明形式提供有关用户的信息：</span><span class="sxs-lookup"><span data-stu-id="964e3-127">It also provides information about the user in the form of claims:</span></span>

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

<span data-ttu-id="964e3-128">详细了解[Azure AD B2C 令牌引用](active-directory-b2c-reference-tokens.md)中可用于应用程序的令牌类型和声明。</span><span class="sxs-lookup"><span data-stu-id="964e3-128">Learn more about the types of tokens and claims available to an application in the [Azure AD B2C token reference](active-directory-b2c-reference-tokens.md).</span></span>

<span data-ttu-id="964e3-129">在 web 应用程序中，每次执行[策略](active-directory-b2c-reference-policies.md)都要执行以下高级步骤：</span><span class="sxs-lookup"><span data-stu-id="964e3-129">In a web application, each execution of a [policy](active-directory-b2c-reference-policies.md) takes these high-level steps:</span></span>

1. <span data-ttu-id="964e3-130">用户浏览到 web 应用程序。</span><span class="sxs-lookup"><span data-stu-id="964e3-130">The user browses to the web application.</span></span>
2. <span data-ttu-id="964e3-131">Web 应用程序将用户重定向到 Azure AD B2C，以指示要执行的策略。</span><span class="sxs-lookup"><span data-stu-id="964e3-131">The web application redirects the user to Azure AD B2C indicating the policy to execute.</span></span>
3. <span data-ttu-id="964e3-132">用户完成策略。</span><span class="sxs-lookup"><span data-stu-id="964e3-132">The user completes policy.</span></span>
4. <span data-ttu-id="964e3-133">Azure AD B2C 在浏览器中返回 @no__t 0。</span><span class="sxs-lookup"><span data-stu-id="964e3-133">Azure AD B2C returns an `id_token` to the browser.</span></span>
5. <span data-ttu-id="964e3-134">@No__t 将发布到重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="964e3-134">The `id_token` is posted to the redirect URI.</span></span>
6. <span data-ttu-id="964e3-135">验证 `id_token` 并设置会话 cookie。</span><span class="sxs-lookup"><span data-stu-id="964e3-135">The `id_token` is validated and a session cookie is set.</span></span>
7. <span data-ttu-id="964e3-136">将向用户返回一个安全页。</span><span class="sxs-lookup"><span data-stu-id="964e3-136">A secure page is returned to the user.</span></span>

<span data-ttu-id="964e3-137">使用从 Azure AD 接收的公共签名密钥验证 `id_token` 足以验证用户的身份。</span><span class="sxs-lookup"><span data-stu-id="964e3-137">Validation of the `id_token` by using a public signing key that is received from Azure AD is sufficient to verify the identity of the user.</span></span> <span data-ttu-id="964e3-138">此过程还会设置会话 cookie，可用于在后续页面请求中标识用户。</span><span class="sxs-lookup"><span data-stu-id="964e3-138">This process also sets a session cookie that can be used to identify the user on subsequent page requests.</span></span>

<span data-ttu-id="964e3-139">若要查看此方案的运行情况，请尝试在 "入门"[部分](active-directory-b2c-overview.md)中提供 web 应用程序登录代码示例之一。</span><span class="sxs-lookup"><span data-stu-id="964e3-139">To see this scenario in action, try one of the web application sign-in code samples in our [Getting started section](active-directory-b2c-overview.md).</span></span>

<span data-ttu-id="964e3-140">除了便于简单登录，web 服务器应用程序还可能需要访问后端 web 服务。</span><span class="sxs-lookup"><span data-stu-id="964e3-140">In addition to facilitating simple sign-in, a web server application might also need to access a back-end web service.</span></span> <span data-ttu-id="964e3-141">在这种情况下，web 应用程序可以执行略有不同的[OpenID connect 流](active-directory-b2c-reference-oidc.md)，并使用授权代码和刷新令牌来获取令牌。</span><span class="sxs-lookup"><span data-stu-id="964e3-141">In this case, the web application can perform a slightly different [OpenID Connect flow](active-directory-b2c-reference-oidc.md) and acquire tokens by using authorization codes and refresh tokens.</span></span> <span data-ttu-id="964e3-142">下面的[Web api 部分](#web-apis)描述了此方案。</span><span class="sxs-lookup"><span data-stu-id="964e3-142">This scenario is depicted in the following [Web APIs section](#web-apis).</span></span>

## <a name="web-apis"></a><span data-ttu-id="964e3-143">Web Api</span><span class="sxs-lookup"><span data-stu-id="964e3-143">Web APIs</span></span>

<span data-ttu-id="964e3-144">你可以使用 Azure AD B2C 来保护 web 服务，例如应用程序的 RESTful web API。</span><span class="sxs-lookup"><span data-stu-id="964e3-144">You can use Azure AD B2C to secure web services such as your application's RESTful web API.</span></span> <span data-ttu-id="964e3-145">Web Api 可以使用 OAuth 2.0 通过使用令牌对传入的 HTTP 请求进行身份验证来保护其数据。</span><span class="sxs-lookup"><span data-stu-id="964e3-145">Web APIs can use OAuth 2.0 to secure their data, by authenticating incoming HTTP requests using tokens.</span></span> <span data-ttu-id="964e3-146">Web API 的调用方在 HTTP 请求的授权标头中追加一个标记：</span><span class="sxs-lookup"><span data-stu-id="964e3-146">The caller of a web API appends a token in the authorization header of an HTTP request:</span></span>

```
GET /api/items HTTP/1.1
Host: www.mywebapi.com
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6...
Accept: application/json
...
```

<span data-ttu-id="964e3-147">然后，web API 可以使用令牌来验证 API 调用方的标识，并从令牌中编码的声明提取有关调用方的信息。</span><span class="sxs-lookup"><span data-stu-id="964e3-147">The web API can then use the token to verify the API caller's identity and to extract information about the caller from claims that are encoded in the token.</span></span> <span data-ttu-id="964e3-148">详细了解[Azure AD B2C 令牌参考](active-directory-b2c-reference-tokens.md)中的应用可用的令牌和声明类型。</span><span class="sxs-lookup"><span data-stu-id="964e3-148">Learn more about the types of tokens and claims available to an app in the [Azure AD B2C token reference](active-directory-b2c-reference-tokens.md).</span></span>

<span data-ttu-id="964e3-149">Web API 可以从许多类型的客户端（包括 web 应用程序、桌面和移动应用程序、单页应用程序、服务器端守护程序以及其他 web Api）接收令牌。</span><span class="sxs-lookup"><span data-stu-id="964e3-149">A web API can receive tokens from many types of clients, including web applications, desktop and mobile applications, single page applications, server-side daemons, and other web APIs.</span></span> <span data-ttu-id="964e3-150">下面是用于调用 web API 的 web 应用程序的完整流示例：</span><span class="sxs-lookup"><span data-stu-id="964e3-150">Here's an example of the complete flow for a web application that calls a web API:</span></span>

1. <span data-ttu-id="964e3-151">Web 应用程序执行策略，用户完成用户体验。</span><span class="sxs-lookup"><span data-stu-id="964e3-151">The web application executes a policy and the user completes the user experience.</span></span>
2. <span data-ttu-id="964e3-152">Azure AD B2C 返回（OpenID Connect） `id_token`，并向浏览器返回一个授权代码。</span><span class="sxs-lookup"><span data-stu-id="964e3-152">Azure AD B2C returns an (OpenID Connect) `id_token` and an authorization code to the browser.</span></span>
3. <span data-ttu-id="964e3-153">浏览器将 @no__t 0 和授权代码发送到重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="964e3-153">The browser posts the `id_token` and authorization code to the redirect URI.</span></span>
4. <span data-ttu-id="964e3-154">Web 服务器验证 `id_token` 并设置会话 cookie。</span><span class="sxs-lookup"><span data-stu-id="964e3-154">The web server validates the `id_token` and sets a session cookie.</span></span>
5. <span data-ttu-id="964e3-155">Web 服务器通过向其提供授权代码、应用程序客户端 ID 和客户端凭据来请求 @no__t Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="964e3-155">The web server asks Azure AD B2C for an `access_token` by providing it with the authorization code, application client ID, and client credentials.</span></span>
6. <span data-ttu-id="964e3-156">将 `access_token` 和 `refresh_token` 返回到 web 服务器。</span><span class="sxs-lookup"><span data-stu-id="964e3-156">The `access_token` and `refresh_token` are returned to the web server.</span></span>
7. <span data-ttu-id="964e3-157">使用授权标头中的 `access_token` 调用 web API。</span><span class="sxs-lookup"><span data-stu-id="964e3-157">The web API is called with the `access_token` in an authorization header.</span></span>
8. <span data-ttu-id="964e3-158">Web API 将验证令牌。</span><span class="sxs-lookup"><span data-stu-id="964e3-158">The web API validates the token.</span></span>
9. <span data-ttu-id="964e3-159">安全数据将返回到 web 应用程序。</span><span class="sxs-lookup"><span data-stu-id="964e3-159">Secure data is returned to the web application.</span></span>

<span data-ttu-id="964e3-160">若要详细了解授权代码、刷新令牌和获取令牌的步骤，请参阅[OAuth 2.0 协议](active-directory-b2c-reference-oauth-code.md)。</span><span class="sxs-lookup"><span data-stu-id="964e3-160">To learn more about authorization codes, refresh tokens, and the steps for getting tokens, read about the [OAuth 2.0 protocol](active-directory-b2c-reference-oauth-code.md).</span></span>

<span data-ttu-id="964e3-161">若要了解如何使用 Azure AD B2C 保护 web API，请参阅[入门部分](active-directory-b2c-overview.md)中的 web api 教程。</span><span class="sxs-lookup"><span data-stu-id="964e3-161">To learn how to secure a web API by using Azure AD B2C, check out the web API tutorials in our [Getting started section](active-directory-b2c-overview.md).</span></span>

## <a name="mobile-and-native-applications"></a><span data-ttu-id="964e3-162">移动和本机应用程序</span><span class="sxs-lookup"><span data-stu-id="964e3-162">Mobile and native applications</span></span>

<span data-ttu-id="964e3-163">安装在设备上的应用程序（如移动和桌面应用程序）通常需要代表用户访问后端服务或 web Api。</span><span class="sxs-lookup"><span data-stu-id="964e3-163">Applications that are installed on devices, such as mobile and desktop applications, often need to access back-end services or web APIs on behalf of users.</span></span> <span data-ttu-id="964e3-164">你可以通过使用 Azure AD B2C 和[OAuth 2.0 授权代码流](active-directory-b2c-reference-oauth-code.md)，将自定义的标识管理体验添加到本机应用程序并安全调用后端服务。</span><span class="sxs-lookup"><span data-stu-id="964e3-164">You can add customized identity management experiences to your native applications and securely call back-end services by using Azure AD B2C and the [OAuth 2.0 authorization code flow](active-directory-b2c-reference-oauth-code.md).</span></span>

<span data-ttu-id="964e3-165">在此流中，应用程序执行[策略](active-directory-b2c-reference-policies.md)，并在用户完成策略后从 Azure AD 接收 @no__t。</span><span class="sxs-lookup"><span data-stu-id="964e3-165">In this flow, the application executes [policies](active-directory-b2c-reference-policies.md) and receives an `authorization_code` from Azure AD after the user completes the policy.</span></span> <span data-ttu-id="964e3-166">@No__t-0 表示应用程序代表当前登录用户调用后端服务的权限。</span><span class="sxs-lookup"><span data-stu-id="964e3-166">The `authorization_code` represents the application's permission to call back-end services on behalf of the user who is currently signed in.</span></span> <span data-ttu-id="964e3-167">然后，应用程序可以在后台为 @no__t 和 @no__t 交换 `authorization_code`。</span><span class="sxs-lookup"><span data-stu-id="964e3-167">The application can then exchange the `authorization_code` in the background for an `access_token` and a `refresh_token`.</span></span>  <span data-ttu-id="964e3-168">应用程序可以使用 `access_token` 向 HTTP 请求中的后端 web API 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="964e3-168">The application can use the `access_token` to authenticate to a back-end web API in HTTP requests.</span></span> <span data-ttu-id="964e3-169">它还可以使用 `refresh_token` 在旧的 @no__t 过期时获取新的。</span><span class="sxs-lookup"><span data-stu-id="964e3-169">It can also use the `refresh_token` to get a new `access_token` when an older one expires.</span></span>

## <a name="current-limitations"></a><span data-ttu-id="964e3-170">当前限制</span><span class="sxs-lookup"><span data-stu-id="964e3-170">Current limitations</span></span>

### <a name="unsupported-application-types"></a><span data-ttu-id="964e3-171">不受支持的应用程序类型</span><span class="sxs-lookup"><span data-stu-id="964e3-171">Unsupported application types</span></span>

#### <a name="daemonsserver-side-applications"></a><span data-ttu-id="964e3-172">守护程序/服务器端应用程序</span><span class="sxs-lookup"><span data-stu-id="964e3-172">Daemons/server-side applications</span></span>

<span data-ttu-id="964e3-173">包含长时间运行的进程或在没有用户的情况下运行的应用程序还需要通过某种方式来访问受保护的资源（如 web Api）。</span><span class="sxs-lookup"><span data-stu-id="964e3-173">Applications that contain long-running processes or that operate without the presence of a user also need a way to access secured resources such as web APIs.</span></span> <span data-ttu-id="964e3-174">这些应用程序可以通过使用应用程序的标识（而不是用户的委派标识）和 OAuth 2.0 客户端凭据流来对令牌进行身份验证和获取令牌。</span><span class="sxs-lookup"><span data-stu-id="964e3-174">These applications can authenticate and get tokens by using the application's identity (rather than a user's delegated identity) and by using the OAuth 2.0 client credentials flow.</span></span> <span data-ttu-id="964e3-175">客户端凭据流不同于代表流，而且不应用于服务器到服务器的身份验证流。</span><span class="sxs-lookup"><span data-stu-id="964e3-175">Client credential flow is not the same as on-behalf-flow and on-behalf-flow should not be used for server-to-server authentication.</span></span>

<span data-ttu-id="964e3-176">尽管 Azure AD B2C 当前不支持客户端凭据流，但你可以使用 Azure AD 设置客户端凭据流。</span><span class="sxs-lookup"><span data-stu-id="964e3-176">Although client credential flow is not currently supported by Azure AD B2C, you can set up client credential flow using Azure AD.</span></span> <span data-ttu-id="964e3-177">Azure AD B2C 租户与 Azure AD 企业租户共享某些功能。</span><span class="sxs-lookup"><span data-stu-id="964e3-177">An Azure AD B2C tenant shares some functionality with Azure AD enterprise tenants.</span></span>  <span data-ttu-id="964e3-178">使用 Azure AD B2C 租户的 Azure AD 功能支持客户端凭据流。</span><span class="sxs-lookup"><span data-stu-id="964e3-178">The client credential flow is supported using the Azure AD functionality of the Azure AD B2C tenant.</span></span>

<span data-ttu-id="964e3-179">若要设置客户端凭据流，请参阅[Azure Active Directory v2.0 和 OAuth 2.0 客户端凭据流](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds)。</span><span class="sxs-lookup"><span data-stu-id="964e3-179">To set up client credential flow, see [Azure Active Directory v2.0 and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds).</span></span> <span data-ttu-id="964e3-180">身份验证成功后，将收到已设置格式的令牌，以便 Azure AD 如[Azure AD 令牌参考](https://docs.microsoft.com/azure/active-directory/develop/active-directory-token-and-claims)中所述。</span><span class="sxs-lookup"><span data-stu-id="964e3-180">A successful authentication results in the receipt of a token formatted so that it can be used by Azure AD as described in [Azure AD token reference](https://docs.microsoft.com/azure/active-directory/develop/active-directory-token-and-claims).</span></span>

#### <a name="web-api-chains-on-behalf-of-flow"></a><span data-ttu-id="964e3-181">Web API 链（代理流）</span><span class="sxs-lookup"><span data-stu-id="964e3-181">Web API chains (on-behalf-of flow)</span></span>

<span data-ttu-id="964e3-182">许多体系结构包含需要调用另一个下游 web API 的 web API，这两者都受 Azure AD B2C 保护。</span><span class="sxs-lookup"><span data-stu-id="964e3-182">Many architectures include a web API that needs to call another downstream web API, where both are secured by Azure AD B2C.</span></span> <span data-ttu-id="964e3-183">此方案常见于具有 Web API 后端的本机客户端，并调用 Microsoft online 服务（例如 Azure AD 图形 API）。</span><span class="sxs-lookup"><span data-stu-id="964e3-183">This scenario is common in native clients that have a Web API back-end and calls a Microsoft online service such as the Azure AD Graph API.</span></span>

<span data-ttu-id="964e3-184">可以通过使用 OAuth 2.0 JWT 持有者凭据授权（也称为代理流）来支持这种链接的 web API 方案。</span><span class="sxs-lookup"><span data-stu-id="964e3-184">This chained web API scenario can be supported by using the OAuth 2.0 JWT bearer credential grant, also known as the on-behalf-of flow.</span></span>  <span data-ttu-id="964e3-185">但 Azure AD B2C 中当前未实现代理流。</span><span class="sxs-lookup"><span data-stu-id="964e3-185">However, the on-behalf-of flow is not currently implemented in the Azure AD B2C.</span></span>

### <a name="faulted-apps"></a><span data-ttu-id="964e3-186">出错的应用</span><span class="sxs-lookup"><span data-stu-id="964e3-186">Faulted apps</span></span>

<span data-ttu-id="964e3-187">不要通过以下方式编辑 Azure AD B2C 应用程序：</span><span class="sxs-lookup"><span data-stu-id="964e3-187">Do not edit Azure AD B2C applications in these ways:</span></span>

- <span data-ttu-id="964e3-188">在其他应用程序管理门户上，如[应用程序注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)。</span><span class="sxs-lookup"><span data-stu-id="964e3-188">On other application management portals such as the [Application Registration Portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
- <span data-ttu-id="964e3-189">使用图形 API 或 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="964e3-189">Using Graph API or PowerShell.</span></span>

<span data-ttu-id="964e3-190">如果在 Azure 门户之外编辑 Azure AD B2C 应用程序，则该应用程序将成为出错的应用程序，并且不能再与 Azure AD B2C 一起使用。</span><span class="sxs-lookup"><span data-stu-id="964e3-190">If you edit the Azure AD B2C application outside of the Azure portal, it becomes a faulted application and is no longer usable with Azure AD B2C.</span></span> <span data-ttu-id="964e3-191">删除并重新创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="964e3-191">Delete the application and create it again.</span></span>

<span data-ttu-id="964e3-192">若要删除应用程序，请在[应用程序注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中，并删除该应用程序。</span><span class="sxs-lookup"><span data-stu-id="964e3-192">To delete the application, go to the [Application Registration Portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade) and delete the application there.</span></span> <span data-ttu-id="964e3-193">为了使应用程序可见，你需要是应用程序的所有者（而不只是租户的管理员）。</span><span class="sxs-lookup"><span data-stu-id="964e3-193">In order for the application to be visible, you need to be the owner of the application (and not just an admin of the tenant).</span></span>

## <a name="next-steps"></a><span data-ttu-id="964e3-194">后续步骤</span><span class="sxs-lookup"><span data-stu-id="964e3-194">Next steps</span></span>

<span data-ttu-id="964e3-195">了解有关[Azure Active Directory B2C 中的用户流](active-directory-b2c-reference-policies.md)提供的内置策略的详细信息。</span><span class="sxs-lookup"><span data-stu-id="964e3-195">Find out more about the built-in policies provided by [User flows in Azure Active Directory B2C](active-directory-b2c-reference-policies.md).</span></span>
