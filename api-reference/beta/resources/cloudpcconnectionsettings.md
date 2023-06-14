---
title: "cloudPcConnectionSettings resource type"
description: "Represents the details of the Cloud PC connection settings."
author: "xumzheng"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: resourcePageType
---

# cloudPcConnectionSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The connection settings of a Cloud PC. Currently, only enableSinleSignOn is supported. IT admin could enable it through updating provisioning policy and calling applyConfig/apply API.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|enableSingleSignOn|Boolean|When `true`, indicates the single sign on is enabled. When `false` indicates single sign on is disabled. default value is `false`. |

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcConnectionSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcConnectionSettings",
  "enableSingleSignOn": true
}
```