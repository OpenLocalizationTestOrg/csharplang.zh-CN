---
title: 使用 Azure 顾问降低服务成本 |Microsoft Docs
description: 使用 Azure 顾问优化 Azure 部署的成本。
services: advisor
documentationcenter: NA
author: kasparks
ms.service: advisor
ms.topic: article
ms.date: 01/29/2019
ms.author: kasparks
ms.openlocfilehash: 34031883ec432fce4dcdcd3e825c99e453a6c6e3
ms.sourcegitcommit: 5aca2af2f2c521ae3f3e7fab640edda966edd007
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "6610196"
---
![Test1noicon](./image/Test1noicon.png)

# <a name="reduce-service-costs-using-azure-advisor"></a>使用 Azure 顾问降低服务成本

顾问通过识别空闲和未充分利用的资源，帮助你优化和减少总体 Azure 支出。 可以从顾问仪表板上的 "**成本**" 选项卡获取成本建议。 这是测试123。

## <a name="optimize-virtual-machine-spend-by-resizing-or-shutting-down-underutilized-instances"></a>通过调整大小或关闭未充分利用的实例来优化虚拟机花费 

虽然某些应用程序方案在设计上可能导致低利用率，但你通常可以通过管理虚拟机的大小和数量来节省资金。 Advisor 会监视你的虚拟机使用情况7天，然后标识低利用率虚拟机。 如果虚拟机的 CPU 利用率为5% 或更低，并且其网络利用率小于2%，或者当前工作负荷可由较小的虚拟机大小容纳，则会将虚拟机视为低利用率。这是不是就地测试。

顾问会显示继续运行虚拟机所需的估计成本，以便可以选择关闭虚拟机或调整其大小。

如果你想要更积极地识别使用不足的虚拟机，你可以基于每个订阅调整平均 CPU 使用率规则。

## <a name="reduce-costs-by-eliminating-unprovisioned-expressroute-circuits"></a>消除未设置的 ExpressRoute 线路，从而降低成本

顾问会确定提供程序状态为 "*未设置*" 的 ExpressRoute 线路超过一个月，如果不打算使用连接服务提供商来预配线路，则建议删除该线路。

## <a name="reduce-costs-by-deleting-or-reconfiguring-idle-virtual-network-gateways"></a>删除或重新配置空闲虚拟网络网关，降低成本

顾问标识在超过90天内空闲的虚拟网络入口。 由于这些网关按小时计费，因此，如果不想再使用它们，则应考虑重新配置或删除它们。 

## <a name="buy-reserved-virtual-machine-instances-to-save-money-over-pay-as-you-go-costs"></a>购买保留虚拟机实例，通过即用即付成本节省资金

Advisor 将在过去30天内检查虚拟机的使用情况，并确定是否可以通过购买 Azure 保留来节省资金。 顾问会向你显示最大限度地节省费用的区域和大小，并将向你显示购买预留的估计节省量。 借助 Azure 保留，你可以为虚拟机预先购买基本成本。 折扣将自动应用于与预留大小和区域相同的新的或现有的 Vm。 [详细了解 Azure 保留 VM 实例。](https://azure.microsoft.com/pricing/reserved-vm-instances/)

顾问还会通知你你的保留实例将在未来30天到期。 建议你购买新的预订实例，以避免支付即用即付定价。

## <a name="delete-unassociated-public-ip-addresses-to-save-money"></a>删除未关联的公共 IP 地址以节省资金

顾问标识当前不与 Azure 资源（例如负载均衡器或 Vm）关联的公共 IP 地址。 这些公共 IP 地址附带了一个名义费用。 如果你不打算使用它们，则删除它们可能会节省成本。

## <a name="how-to-access-cost-recommendations-in-azure-advisor"></a>如何访问 Azure 顾问中的成本建议

:::image type="complex"  alt-text="这是一个用于 contoso-scope1 的复杂映像测试功能" loc-scope="Azure" source="./Test.png"::: 
这是针对 contoso-scope1 的复杂映像测试功能的日志说明，这是多行 testing1 :::image-end:::

1. 登录到[Azure 门户](https://portal.azure.com)，然后打开[Advisor](https://aka.ms/azureadvisordashboard)。
:::icon source="image\Test123.png":::这是图标源测试，这是下一行的测试

2.  在顾问仪表板上，单击 "**成本**" 选项卡。这是一个 :::no-loc text="TEST for inline lock":::，用于查看是否将删除 "测试内联位置" 或将其作为标记进行放置。

:::image source="https://portal.azure.com" alt-text="这是图像源测试":::
TLong 说明开始。顾问标识当前不与 Azure 资源（例如负载均衡器或 Vm）关联的公共 IP 地址。 这些公共 IP 地址附带了一个名义费用。 如果你不打算使用它们，则删除它们可能会节省成本。
长说明结束 :::image-end:::这是图像结束

::: image source= "./image/Test1noicon.png" alt-text="space teating":::

:::image type="complex" source="./image/Test1noicon.png" alt-text="这是一个用于 contoso-scope2 的复杂映像测试功能" loc-scope="Azure"::: 
这是针对 contoso-scope2 的复杂映像测试功能的日志说明，这是多行 testing2 :::image-end:::

## <a name="next-steps"></a>后续步骤

若要了解有关顾问建议的详细信息，请参阅：
* [Advisor 简介](advisor-overview.md)
* [入门](advisor-get-started.md)
* [顾问性能建议](advisor-cost-recommendations.md)
* [顾问高可用性建议](advisor-cost-recommendations.md)
* [顾问安全建议](advisor-cost-recommendations.md)
