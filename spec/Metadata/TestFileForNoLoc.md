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
- virtual machine
ms.openlocfilehash: 734f2a23565edfe472b9732f724501cdfbd44995
ms.sourcegitcommit: 9ff95935fb1f4654097b87b1105fd7358ac93a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2019
ms.locfileid: "67540135"
---
# <a name="reduce-service-costs-using-azure-opno-locadvisor"></a><span data-ttu-id="6dad2-103">降低服务成本使用 Azure Advisor</span><span class="sxs-lookup"><span data-stu-id="6dad2-103">Reduce service costs using Azure Advisor</span></span>

Advisor<span data-ttu-id="6dad2-104"> 可帮助你优化并降低 Azure 总支出通过识别闲置和未充分利用资源。</span><span class="sxs-lookup"><span data-stu-id="6dad2-104"> helps you optimize and reduce your overall Azure spend by identifying idle and underutilized resources.</span></span> <span data-ttu-id="6dad2-105">你可以获取成本建议**成本**选项卡上Advisor仪表板。</span><span class="sxs-lookup"><span data-stu-id="6dad2-105">You can get cost recommendations from the **Cost** tab on the Advisor dashboard.</span></span> <span data-ttu-id="6dad2-106">这是测试 123。</span><span class="sxs-lookup"><span data-stu-id="6dad2-106">This is TEST 123.</span></span>

## <a name="optimize-opno-locvirtual-machine-spend-by-resizing-or-shutting-down-underutilized-instances"></a><span data-ttu-id="6dad2-107">优化virtual machine花费通过调整或关闭未充分利用的实例</span><span class="sxs-lookup"><span data-stu-id="6dad2-107">Optimize virtual machine spend by resizing or shutting down underutilized instances</span></span> 

<span data-ttu-id="6dad2-108">虽然某些应用程序方案会根据设计利用率较低，但通常可以通过管理的大小和数量来节省资金你virtual machines。</span><span class="sxs-lookup"><span data-stu-id="6dad2-108">Although certain application scenarios can result in low utilization by design, you can often save money by managing the size and number of your virtual machines.</span></span> Advisor<span data-ttu-id="6dad2-109"> 监视你virtual machine7 天的使用情况，然后标识利用率较低的virtual machines。</span><span class="sxs-lookup"><span data-stu-id="6dad2-109"> monitors your virtual machine usage for 7 days and then identifies low-utilization virtual machines.</span></span> <span data-ttu-id="6dad2-110">虚拟机被视为利用率较低的如果其 CPU 使用率为 5%或更少并且其网络利用率为小于 2%或当前工作负荷是否可以容纳的较小virtual machine大小。这是无 loc 测试。</span><span class="sxs-lookup"><span data-stu-id="6dad2-110">Virtual machines are considered low-utilization if their CPU utilization is 5% or less and their network utilization is less than 2% or if the current workload can be accommodated by a smaller virtual machine size.This is no-loc test.</span></span>

Advisor<span data-ttu-id="6dad2-111"> 会显示继续运行的估计的成本将virtual machine，以便您可以选择将其关闭或重设其大小。</span><span class="sxs-lookup"><span data-stu-id="6dad2-111"> shows you the estimated cost of continuing to run your virtual machine, so that you can choose to shut it down or resize it.</span></span>

<span data-ttu-id="6dad2-112">如果你想要加强的标识未充分利用virtual machines，可以调整平均 CPU 使用率规则基于每个订阅。</span><span class="sxs-lookup"><span data-stu-id="6dad2-112">If you want to be more aggressive at identifying underutilized virtual machines, you can adjust the average CPU utilization rule on a per subscription basis.</span></span>

## <a name="reduce-costs-by-eliminating-unprovisioned-expressroute-circuits"></a><span data-ttu-id="6dad2-113">通过消除未设置的 ExpressRoute 线路来降低成本</span><span class="sxs-lookup"><span data-stu-id="6dad2-113">Reduce costs by eliminating unprovisioned ExpressRoute circuits</span></span>

Advisor<span data-ttu-id="6dad2-114"> 标识已的提供程序状态的 ExpressRoute 线路*未预配*为超过一个月，将建议删除该线路，如果你不打算使用连接服务提供商预配线路。</span><span class="sxs-lookup"><span data-stu-id="6dad2-114"> identifies ExpressRoute circuits that have been in the provider status of *Not Provisioned* for more than one month, and recommends deleting the circuit if you aren't planning to provision the circuit with your connectivity provider.</span></span>

## <a name="reduce-costs-by-deleting-or-reconfiguring-idle-virtual-network-gateways"></a><span data-ttu-id="6dad2-115">通过删除或重新配置空闲虚拟网络网关来降低成本</span><span class="sxs-lookup"><span data-stu-id="6dad2-115">Reduce costs by deleting or reconfiguring idle virtual network gateways</span></span>

Advisor<span data-ttu-id="6dad2-116"> 标识已空闲时间超过 90 天的虚拟网络入口。</span><span class="sxs-lookup"><span data-stu-id="6dad2-116"> identifies virtual network gates that have been idle for over 90 days.</span></span> <span data-ttu-id="6dad2-117">由于这些网关按小时计费，因此如果不打算再使用它们，则应考虑重新配置或删除它们。</span><span class="sxs-lookup"><span data-stu-id="6dad2-117">Since these gateways are billed hourly, you should consider reconfiguring or deleting them if you don't intend to use them anymore.</span></span> 

## <a name="buy-reserved-opno-locvirtual-machine-instances-to-save-money-over-pay-as-you-go-costs"></a><span data-ttu-id="6dad2-118">购买保留virtual machine实例可节省即用即付成本</span><span class="sxs-lookup"><span data-stu-id="6dad2-118">Buy reserved virtual machine instances to save money over pay-as-you-go costs</span></span>

Advisor<span data-ttu-id="6dad2-119"> 将查看你virtual machine最近 30 天内的使用情况，并确定是否无法通过购买 Azure 预订节省资金。</span><span class="sxs-lookup"><span data-stu-id="6dad2-119"> will review your virtual machine usage over the last 30 days and determine if you could save money by purchasing an Azure reservation.</span></span> Advisor<span data-ttu-id="6dad2-120"> 将显示的区域和大小可能具有的大多数节约和显示与购买的预订的估计的节约。</span><span class="sxs-lookup"><span data-stu-id="6dad2-120"> will show you the regions and sizes where you potentially have the most savings and will show you the estimated savings from purchasing reservations.</span></span> <span data-ttu-id="6dad2-121">通过 Azure 保留项，你可以预先购买的基本费用在virtual machines。</span><span class="sxs-lookup"><span data-stu-id="6dad2-121">With Azure reservations, you can pre-purchase the base costs for your virtual machines.</span></span> <span data-ttu-id="6dad2-122">折扣将自动应用于新的或现有的 VM，这些 VM 具有与预留相同的大小和区域。</span><span class="sxs-lookup"><span data-stu-id="6dad2-122">Discounts will automatically apply to new or existing VMs that have the same size and region as your reservations.</span></span> [<span data-ttu-id="6dad2-123">深入了解 Azure 虚拟机预留实例。</span><span class="sxs-lookup"><span data-stu-id="6dad2-123">Learn more about Azure Reserved VM Instances.</span></span>](https://azure.microsoft.com/pricing/reserved-vm-instances/)

Advisor<span data-ttu-id="6dad2-124"> 将也会通知你的预订实例都可以将在接下来的 30 天后过期。</span><span class="sxs-lookup"><span data-stu-id="6dad2-124"> will also notify you of reserved instances that you have that will expire in the next 30 days.</span></span> <span data-ttu-id="6dad2-125">它将建议你购买新的预留实例来避免即用即付定价。</span><span class="sxs-lookup"><span data-stu-id="6dad2-125">It will recommend that you purchase new reserved instances to avoid paying pay-as-you-go pricing.</span></span>

## <a name="delete-unassociated-public-ip-addresses-to-save-money"></a><span data-ttu-id="6dad2-126">删除未关联的公共 IP 地址可节省资金</span><span class="sxs-lookup"><span data-stu-id="6dad2-126">Delete unassociated public IP addresses to save money</span></span>

Advisor<span data-ttu-id="6dad2-127"> 标识不是当前关联到负载均衡器或虚拟机等 Azure 资源的公共 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="6dad2-127"> identifies public IP addresses that are not currently associated to Azure resources such as Load Balancers or VMs.</span></span> <span data-ttu-id="6dad2-128">这些公共 IP 地址会产生少许费用。</span><span class="sxs-lookup"><span data-stu-id="6dad2-128">These public IP addresses come with a nominal charge.</span></span> <span data-ttu-id="6dad2-129">如果不打算使用它们，删除它们可以节省成本。</span><span class="sxs-lookup"><span data-stu-id="6dad2-129">If you do not plan to use them, deleting them can result in cost savings.</span></span>

## <a name="how-to-access-cost-recommendations-in-azure-opno-locadvisor"></a><span data-ttu-id="6dad2-130">如何访问 Azure 中的成本建议 Advisor</span><span class="sxs-lookup"><span data-stu-id="6dad2-130">How to access Cost recommendations in Azure Advisor</span></span>

1. <span data-ttu-id="6dad2-131">登录到[Azure 门户](https://portal.azure.com)，然后打开[ Advisor ](https://aka.ms/azureadvisordashboard)。</span><span class="sxs-lookup"><span data-stu-id="6dad2-131">Sign in to the [Azure portal](https://portal.azure.com), and then open [Advisor](https://aka.ms/azureadvisordashboard).</span></span>

2.  <span data-ttu-id="6dad2-132">上Advisor仪表板中，单击**成本**选项卡。这是:::no-loc text="TEST for inline lock":::以查看是否将删除或标记作为内联 loc 的"测试"。</span><span class="sxs-lookup"><span data-stu-id="6dad2-132">On the Advisor dashboard, click the **Cost** tab. This is a :::no-loc text="TEST for inline lock"::: to see if the "TEST for inline loc" will be removed or put as a tag.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6dad2-133">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6dad2-133">Next steps</span></span>

<span data-ttu-id="6dad2-134">若要详细了解Advisor的建议，请参阅：</span><span class="sxs-lookup"><span data-stu-id="6dad2-134">To learn more about Advisor recommendations, see:</span></span>
* <span data-ttu-id="6dad2-135">[简介 Advisor](advisor-overview.md)</span><span class="sxs-lookup"><span data-stu-id="6dad2-135">[Introduction to Advisor](advisor-overview.md)</span></span>
* [<span data-ttu-id="6dad2-136">入门</span><span class="sxs-lookup"><span data-stu-id="6dad2-136">Get Started</span></span>](advisor-get-started.md)
* <span data-ttu-id="6dad2-137">[Advisor 性能建议](advisor-cost-recommendations.md)</span><span class="sxs-lookup"><span data-stu-id="6dad2-137">[Advisor Performance recommendations](advisor-cost-recommendations.md)</span></span>
* <span data-ttu-id="6dad2-138">[Advisor 高可用性建议](advisor-cost-recommendations.md)</span><span class="sxs-lookup"><span data-stu-id="6dad2-138">[Advisor High Availability recommendations](advisor-cost-recommendations.md)</span></span>
* <span data-ttu-id="6dad2-139">[Advisor 安全建议](advisor-cost-recommendations.md)</span><span class="sxs-lookup"><span data-stu-id="6dad2-139">[Advisor Security recommendations](advisor-cost-recommendations.md)</span></span>
