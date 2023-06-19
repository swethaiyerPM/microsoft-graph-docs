---
title: "security resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# security resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [microsoft.graph.entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List securities](../api/user-list-security.md)|[microsoft.graph.security.security](../resources/security-security.md) collection|Get a list of the [microsoft.graph.security.security](../resources/security-security.md) objects and their properties.|
|[Create security](../api/user-post-security.md)|[microsoft.graph.security.security](../resources/security-security.md)|Create a new [microsoft.graph.security.security](../resources/security-security.md) object.|
|[Get security](../api/security-security-get.md)|[microsoft.graph.security.security](../resources/security-security.md)|Read the properties and relationships of a [microsoft.graph.security.security](../resources/security-security.md) object.|
|[Update security](../api/security-security-update.md)|[microsoft.graph.security.security](../resources/security-security.md)|Update the properties of a [microsoft.graph.security.security](../resources/security-security.md) object.|
|[Delete security](../api/user-delete-security.md)|None|Delete a [microsoft.graph.security.security](../resources/security-security.md) object.|
|[List informationProtection](../api/security-security-list-informationprotection.md)|[microsoft.graph.security.informationProtection](../resources/security-informationprotection.md) collection|Get the informationProtection resources from the informationProtection navigation property.|
|[Create informationProtection](../api/security-security-post-informationprotection.md)|[microsoft.graph.security.informationProtection](../resources/security-informationprotection.md)|Create a new informationProtection object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [microsoft.graph.entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|informationProtection|[informationProtection](../resources/security-informationprotection.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.security",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.security",
  "id": "String (identifier)"
}
```

