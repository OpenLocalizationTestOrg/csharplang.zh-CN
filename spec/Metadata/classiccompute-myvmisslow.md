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

# <a name="my-vm-is-slow"></a>我的 VM 运行速度缓慢

尝试执行以下步骤来诊断和解决 VM 性能问题。<br>

## <a name="recommended-steps"></a>**建议的步骤**

1. **您是否知道 PerfInsights 可以帮助你分析 Windows 来宾 VM 问题？**  
    [安装 Azure 性能诊断 VM 扩展](https://docs.microsoft.com/azure/virtual-machines/troubleshooting/performance-diagnostics-vm-extension)直接从 Azure 门户。 你也可以[下载 PerfInsights](https://www.microsoft.com/download/details.aspx?id=54915&fa43d42b-25b5-4a42-fe9b-1634f450f5ee=True)和在 VM 上运行。 若要确保快速解决问题，向我们提供 PerfInsights 日志如果创建支持案例。 [了解更多信息](https://docs.microsoft.com/azure/virtual-machines/troubleshooting/how-to-use-perfInsights)

2. 查看应用程序错误日志、 跟踪和度量值以确定是否有任何应用程序瓶颈造成性能问题。 从一次性问题中恢复的快速方法是，重新启动你的应用程序和虚拟机。

3. 查看操作系统级别指标，如 CPU、 内存使用量、 IO 和网络，以查看是否有任何资源利用率一贯较高。<br>

    上**Windows**，使用[Perfmon](https://docs.microsoft.com/windows-server/administration/windows-commands/perfmon)工具<br>
    上**Linux**，使用 Top、 VmStat、 Lsof 和 Tcpdump 等命令<br>

4. 使用[VM 和存储诊断](http://aka.ms/azurevmperf)在 Azure 门户来识别是否有任何资源被过度使用或受到限制。 然后可以启用诊断和监视 Azure Vm 和存储的问题进行疑难解答。

5. 重新启动 VM，以解决任何 VM 操作系统问题，通过单击重新启动在 VM 资源边栏选项卡的顶部。<br>
6. 在 VM 资源的设置边栏选项卡中单击大小扩展虚拟机的不同 VM 类型或系列以提高性能。<br>
7. 请考虑使用[的 Azure 虚拟机工作负荷的高级存储](https://azure.microsoft.com/documentation/articles/storage-premium-storage-preview-portal/)。<br>

## <a name="recommended-documents"></a>**建议的文档**

* [Azure 存储的详细故障排除](https://azure.microsoft.com/documentation/articles/storage-monitoring-diagnosing-troubleshooting/)
