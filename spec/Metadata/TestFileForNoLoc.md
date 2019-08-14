---
title: 降低服务成本使用 Azure 顾问 |Microsoft Docs
description: 使用 Azure 顾问优化 Azure 部署的成本。
services: advisor
documentationcenter: NA
author: kasparks
ms.service: advisor
ms.topic: article
ms.date: 01/29/2019
ms.author: kasparks
ms.openlocfilehash: 0753d6123bd95fc0fb4820e85bab717603dfa163
ms.sourcegitcommit: afdb017b6e7925572904f2d85d86352f95e336ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "6606363"
---
# <a name="reduce-service-costs-using-azure-advisor"></a>降低服务成本使用 Azure 顾问

顾问可帮助你优化并降低 Azure 总支出通过识别闲置和未充分利用资源。 你可以获取成本建议**成本**顾问仪表板上的选项卡。 这是测试 123。

## <a name="optimize-virtual-machine-spend-by-resizing-or-shutting-down-underutilized-instances"></a>优化虚拟机花费通过调整或关闭未充分利用的实例 

虽然某些应用程序方案会根据设计利用率较低，但通常可通过管理的大小和数量的虚拟机来降低成本。 顾问为 7 天内监视虚拟机使用情况，然后识别出利用率较低的虚拟机。 虚拟机被视为利用率较低的如果其 CPU 使用率为 5%或更少并且其网络利用率为小于 2%或当前工作负荷是否可以容纳的较小的虚拟机大小。这是无 loc 测试。

顾问会显示继续运行你的虚拟机，以便您可以选择将其关闭或重设其大小的估计的开销。

如果你想要加强对未充分利用的虚拟机的标识，可以调整平均 CPU 使用率规则基于每个订阅。

## <a name="reduce-costs-by-eliminating-unprovisioned-expressroute-circuits"></a>通过消除未设置的 ExpressRoute 线路来降低成本

顾问可识别这些实例中的提供程序状态的 ExpressRoute 线路*未预配*为超过一个月，将建议删除该线路，如果你不打算使用的连接设置的线路提供程序。

## <a name="reduce-costs-by-deleting-or-reconfiguring-idle-virtual-network-gateways"></a>通过删除或重新配置空闲虚拟网络网关降低成本

顾问标识已空闲时间超过 90 天的虚拟网络入口。 由于这些网关按小时计费，应考虑重新配置或删除它们，如果不想再使用它们。 

## <a name="buy-reserved-virtual-machine-instances-to-save-money-over-pay-as-you-go-costs"></a>购买保留的虚拟机实例可节省即用即付成本

顾问将过去的 30 天内查看虚拟机使用情况，并确定是否无法通过购买 Azure 预订节省资金。 顾问将显示的区域和大小可能具有的大多数节约和显示与购买的预订的估计的节约。 Azure 预订虚拟机可以预购买基本成本。 折扣将自动应用于新的或现有 Vm，为你保留项具有相同的大小和区域。 [了解 Azure 保留 VM 实例有关的详细信息。](https://azure.microsoft.com/pricing/reserved-vm-instances/)

顾问还会通知你的预订实例都可以将在接下来的 30 天后过期。 它将建议购买新的保留实例，以避免支付即用即付定价。

## <a name="delete-unassociated-public-ip-addresses-to-save-money"></a>删除未关联的公共 IP 地址，以节省资金

顾问标识不是当前关联到负载均衡器或虚拟机等 Azure 资源的公共 IP 地址。 这些公共 IP 地址有少许费用。 如果不打算使用它们，则删除它们可能导致节省成本。

## <a name="how-to-access-cost-recommendations-in-azure-advisor"></a>如何访问 Azure 顾问中的成本建议

1. 登录到[Azure 门户](https://portal.azure.com)，然后打开[顾问](https://aka.ms/azureadvisordashboard)。
:::icon source="image\Test123.png":::这是图标源测试，这是测试下一行

2.  在顾问仪表板，单击**成本**选项卡。这是:::no-loc text="TEST for inline lock":::以查看是否将删除或标记作为内联 loc 的"测试"。

:::image source="https://portal.azure.com" alt-text="这是映像源测试":::
TLong 说明开始。顾问标识不是当前关联到负载均衡器或虚拟机等 Azure 资源的公共 IP 地址。 这些公共 IP 地址有少许费用。 如果不打算使用它们，则删除它们可能导致节省成本。
详细说明最终:::image-end:::这是映像结束

::: image source= "./Test.png" alt-test="space teating":::
## <a name="next-steps"></a>后续步骤

若要了解有关顾问建议的详细信息，请参阅：
* [顾问简介](advisor-overview.md)
* [开始](advisor-get-started.md)
* [顾问性能建议](advisor-cost-recommendations.md)
* [顾问高可用性建议](advisor-cost-recommendations.md)
* [顾问安全性建议](advisor-cost-recommendations.md)
