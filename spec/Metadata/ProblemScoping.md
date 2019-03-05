---
ms.openlocfilehash: 9e09fea1b050d4c81afa91b6d3345847f0496805
ms.sourcegitcommit: 55811c551095ea9ab89baf1144ac0cf7fb1c5df8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57253856"
---
<properties
articleId="problemscopingques-ssl"
pageTitle="SSL"
description="SSL"
supportTopicIds="32630470"
authors="khaled-zayed"
ms.author="khzayed"
selfHelpType="problemScopingQuestions"
productPesIds="16072"
cloudEnvironments="public"
schemaVersion="1"
/>
# <a name="ssl"></a><span data-ttu-id="4f9fb-103">SSL</span><span class="sxs-lookup"><span data-stu-id="4f9fb-103">SSL</span></span>
---
{
    "resourceRequired": false,
    "title": "SSL",
    "fileAttachmentHint": "请附加任何相关日志/屏幕截图",
    "formElements": [
        {
            "id": "problem_start_time",
            "order": 1,
            "controlType": "datetimepicker",
            "displayLabel": "事件时间",
            "required": true
        },
        {
            "id": "2",
            "order": 2,
            "controlType": "dropdown",
            "displayLabel": "使用的应用服务证书 （通过 Azure 门户购买） 或 （从第三方购买） 的外部证书？",
            "watermarkText": "选择一个选项",
            "dropdownOptions": [
                {
                    "value": "App Service Certificate",
                    "text": "应用服务证书"
                },
                {
                    "value": "External certificate",
                    "text": "外部证书"
                }
            ],
            "required": false
        },
        {
            "id": "3",
            "order": 3,
            "controlType": "textbox",
            "displayLabel": "SSL 证书颁发给哪个域？",
            "watermarkText": "...",
            "required": false
        },
        {
            "id": "4",
            "order": 4,
            "controlType": "textbox",
            "displayLabel": "什么是您看看和错误时是否看到它？",
            "watermarkText": "...",
            "required": false
        },
        {
            "id": "problem_description",
            "order": 5,
            "controlType": "multilinetextbox",
            "displayLabel": "详细信息",
            "watermarkText": "提供你看到你的问题包括所有错误消息的其他信息。",
            "required": true,
            "useAsAdditionalDetails": true
        }
    ]
}
---
