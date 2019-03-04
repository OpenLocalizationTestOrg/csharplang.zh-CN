---
ms.openlocfilehash: 132dd1bb13c54b49e54f946e46106ff942a84d0f
ms.sourcegitcommit: fed965b15069147176339f9d0d33ff38f0b95f6a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/23/2019
ms.locfileid: "57253850"
---
<properties
    pageTitle="我的 VM 运行速度缓慢"
    description="我的 VM 运行速度缓慢 "
    service="microsoft.classiccompute"
    resource="virtualmachines"
    authors="ScottAzure"
    ms.author="scotro"
    displayOrder="7"
    selfHelpType="resource"
    supportTopicIds="32628264,32628261,32628277,32628254,32628275,32628268,32628281,32628270"
    resourceTags="windows, linux, windowsSQL, redhat"
    productPesIds="14749,15571,15797,16454"
    cloudEnvironments="public"
    articleId="5b164da5-bc96-47b3-8bd9-74cfcf4db851"
    category="性能"
    searchTags="性能降低，、 vm"
/>

# <a name="my-vm-is-slow"></a><span data-ttu-id="f0949-105">我的 VM 运行速度缓慢</span><span class="sxs-lookup"><span data-stu-id="f0949-105">My VM is slow</span></span>

<span data-ttu-id="f0949-106">尝试执行以下步骤来诊断和解决 VM 性能问题。</span><span class="sxs-lookup"><span data-stu-id="f0949-106">Try the following steps to diagnose and mitigate VM performance issues.</span></span><br>

## <a name="recommended-steps"></a><span data-ttu-id="f0949-107">**建议的步骤**</span><span class="sxs-lookup"><span data-stu-id="f0949-107">**Recommended steps**</span></span>

1. <span data-ttu-id="f0949-108">**您是否知道 PerfInsights 可以帮助你分析 Windows 来宾 VM 问题？**</span><span class="sxs-lookup"><span data-stu-id="f0949-108">**Did you know PerfInsights can help you analyze Windows guest VM issues?**</span></span>  
    <span data-ttu-id="f0949-109">[安装 Azure 性能诊断 VM 扩展](https://docs.microsoft.com/azure/virtual-machines/troubleshooting/performance-diagnostics-vm-extension)直接从 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="f0949-109">[Install Azure Performance Diagnostics VM Extension](https://docs.microsoft.com/azure/virtual-machines/troubleshooting/performance-diagnostics-vm-extension) directly from Azure portal.</span></span> <span data-ttu-id="f0949-110">你也可以[下载 PerfInsights](https://www.microsoft.com/download/details.aspx?id=54915&fa43d42b-25b5-4a42-fe9b-1634f450f5ee=True)和在 VM 上运行。</span><span class="sxs-lookup"><span data-stu-id="f0949-110">You may also [download PerfInsights](https://www.microsoft.com/download/details.aspx?id=54915&fa43d42b-25b5-4a42-fe9b-1634f450f5ee=True) and run on the VM.</span></span> <span data-ttu-id="f0949-111">若要确保快速解决问题，向我们提供 PerfInsights 日志如果创建支持案例。</span><span class="sxs-lookup"><span data-stu-id="f0949-111">To ensure a speedy resolution, provide us the PerfInsights logs if you create a support case.</span></span> [<span data-ttu-id="f0949-112">了解更多信息</span><span class="sxs-lookup"><span data-stu-id="f0949-112">Learn more</span></span>](https://docs.microsoft.com/azure/virtual-machines/troubleshooting/how-to-use-perfInsights)

2. <span data-ttu-id="f0949-113">查看应用程序错误日志、 跟踪和度量值以确定是否有任何应用程序瓶颈造成性能问题。</span><span class="sxs-lookup"><span data-stu-id="f0949-113">Review your application error logs, traces, and metrics to determine if there are any application bottlenecks causing performance issues.</span></span> <span data-ttu-id="f0949-114">从一次性问题中恢复的快速方法是，重新启动你的应用程序和虚拟机。</span><span class="sxs-lookup"><span data-stu-id="f0949-114">As a quick way to recover from one-time issues, restart your application and virtual machine.</span></span>

3. <span data-ttu-id="f0949-115">查看操作系统级别指标，如 CPU、 内存使用量、 IO 和网络，以查看是否有任何资源利用率一贯较高。</span><span class="sxs-lookup"><span data-stu-id="f0949-115">Review operating system level metrics such as CPU, memory usage, IO, and network to see if any resource has consistently high utilization.</span></span><br>

    <span data-ttu-id="f0949-116">上**Windows**，使用[Perfmon](https://docs.microsoft.com/windows-server/administration/windows-commands/perfmon)工具</span><span class="sxs-lookup"><span data-stu-id="f0949-116">On **Windows**, use the [Perfmon](https://docs.microsoft.com/windows-server/administration/windows-commands/perfmon) tool</span></span><br>
    <span data-ttu-id="f0949-117">上**Linux**，使用 Top、 VmStat、 Lsof 和 Tcpdump 等命令</span><span class="sxs-lookup"><span data-stu-id="f0949-117">On **Linux**, use commands such as Top, VmStat, Lsof, and Tcpdump</span></span><br>

4. <span data-ttu-id="f0949-118">使用[VM 和存储诊断](http://aka.ms/azurevmperf)在 Azure 门户来识别是否有任何资源被过度使用或受到限制。</span><span class="sxs-lookup"><span data-stu-id="f0949-118">Use [VM and Storage Diagnostics](http://aka.ms/azurevmperf) in the Azure portal to identify if any resource is being overutilized or throttled.</span></span> <span data-ttu-id="f0949-119">然后可以启用诊断和监视 Azure Vm 和存储的问题进行疑难解答。</span><span class="sxs-lookup"><span data-stu-id="f0949-119">You can then enable diagnostics and monitoring to troubleshoot issues with Azure VMs and Storage.</span></span>

5. <span data-ttu-id="f0949-120">重新启动 VM，以解决任何 VM 操作系统问题，通过单击重新启动在 VM 资源边栏选项卡的顶部。</span><span class="sxs-lookup"><span data-stu-id="f0949-120">Restart the VM to address any VM operating system issues by clicking 'Restart' at the top of the VM resource blade.</span></span><br>
6. <span data-ttu-id="f0949-121">在 VM 资源的设置边栏选项卡中单击大小扩展虚拟机的不同 VM 类型或系列以提高性能。</span><span class="sxs-lookup"><span data-stu-id="f0949-121">Scale up the virtual machine to a different VM type or series for increased performance by clicking 'Size' in the Settings blade of the VM resource.</span></span><br>
7. <span data-ttu-id="f0949-122">请考虑使用[的 Azure 虚拟机工作负荷的高级存储](https://azure.microsoft.com/documentation/articles/storage-premium-storage-preview-portal/)。</span><span class="sxs-lookup"><span data-stu-id="f0949-122">Consider using [Premium Storage for Azure Virtual Machine Workloads](https://azure.microsoft.com/documentation/articles/storage-premium-storage-preview-portal/).</span></span><br>

## <a name="recommended-documents"></a><span data-ttu-id="f0949-123">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="f0949-123">**Recommended documents**</span></span>

* [<span data-ttu-id="f0949-124">Azure 存储的详细故障排除</span><span class="sxs-lookup"><span data-stu-id="f0949-124">Detailed troubleshooting of Azure Storage</span></span>](https://azure.microsoft.com/documentation/articles/storage-monitoring-diagnosing-troubleshooting/)
