---
title: 降低服务成本使用 Azure Advisor |Microsoft Docs
description: 使用 AzureAdvisor来优化 Azure 部署的成本。
services: advisor
documentationcenter: NA
author: kasparks
ms.service: advisor
ms.topic: article
ms.date: 01/29/2019
ms.author: kasparks
no-loc:
- Advisor
- virtual machines
ms.openlocfilehash: d13146bc6b73b19d749be7de064d133d11a8ec6b
ms.sourcegitcommit: 437646cd8c576560592110f7fd868b0b3cf27642
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "66308383"
---
# <a name="reduce-service-costs-using-azure-opno-locadvisor"></a>降低服务成本使用 Azure Advisor

Advisor 可帮助你优化并降低 Azure 总支出通过识别闲置和未充分利用资源。 你可以获取成本建议**成本**选项卡上Advisor仪表板。 这是测试 123。

## <a name="optimize-virtual-machine-spend-by-resizing-or-shutting-down-underutilized-instances"></a>优化虚拟机花费通过调整或关闭未充分利用的实例 

虽然某些应用程序方案会根据设计利用率较低，但通常可以通过管理的大小和数量来节省资金你virtual machines。 Advisor 7 天监视虚拟机使用情况，然后标识利用率较低的virtual machines。 虚拟机被视为利用率较低的如果其 CPU 使用率为 5%或更少并且其网络利用率为小于 2%或当前工作负荷是否可以容纳的较小的虚拟机大小。这是无 loc 测试。

Advisor 会显示继续运行你的虚拟机，以便您可以选择将其关闭或重设其大小的估计的成本。

如果你想要加强的标识未充分利用virtual machines，可以调整平均 CPU 使用率规则基于每个订阅。

## <a name="reduce-costs-by-eliminating-unprovisioned-expressroute-circuits"></a>通过消除未设置的 ExpressRoute 线路来降低成本

Advisor 标识已的提供程序状态的 ExpressRoute 线路*未预配*为超过一个月，将建议删除该线路，如果你不打算使用连接服务提供商预配线路。

## <a name="reduce-costs-by-deleting-or-reconfiguring-idle-virtual-network-gateways"></a>通过删除或重新配置空闲虚拟网络网关降低成本

Advisor 标识已空闲时间超过 90 天的虚拟网络入口。 由于这些网关按小时计费，应考虑重新配置或删除它们，如果不想再使用它们。 

## <a name="buy-reserved-virtual-machine-instances-to-save-money-over-pay-as-you-go-costs"></a>购买保留的虚拟机实例可节省即用即付成本

Advisor 将过去的 30 天内查看你的虚拟机使用情况，并确定是否无法通过购买 Azure 预订节省资金。 Advisor 将显示的区域和大小可能具有的大多数节约和显示与购买的预订的估计的节约。 通过 Azure 保留项，你可以预先购买的基本费用在virtual machines。 折扣将自动应用于新的或现有 Vm，为你保留项具有相同的大小和区域。 [了解 Azure 保留 VM 实例有关的详细信息。](https://azure.microsoft.com/pricing/reserved-vm-instances/)

Advisor 将也会通知你的预订实例都可以将在接下来的 30 天后过期。 它将建议购买新的保留实例，以避免支付即用即付定价。

## <a name="delete-unassociated-public-ip-addresses-to-save-money"></a>删除未关联的公共 IP 地址，以节省资金

Advisor 标识不是当前关联到负载均衡器或虚拟机等 Azure 资源的公共 IP 地址。 这些公共 IP 地址有少许费用。 如果不打算使用它们，则删除它们可能导致节省成本。

## <a name="how-to-access-cost-recommendations-in-azure-opno-locadvisor"></a>如何访问 Azure 中的成本建议 Advisor

1. 登录到[Azure 门户](https://portal.azure.com)，然后打开[ Advisor ](https://aka.ms/azureadvisordashboard)。

2.  上Advisor仪表板中，单击**成本**选项卡。
:::no-loc Test="This is Test String":::
## <a name="next-steps"></a>后续步骤

若要详细了解Advisor的建议，请参阅：
* [简介 Advisor](advisor-overview.md)
* [入门](advisor-get-started.md)
* [Advisor 性能建议](advisor-cost-recommendations.md)
* [Advisor 高可用性建议](advisor-cost-recommendations.md)
* [Advisor 安全建议](advisor-cost-recommendations.md)
