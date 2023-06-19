---
title: "auditCoreRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# auditCoreRoot resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [microsoft.graph.entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List auditCoreRoots](../api/security-security-list-auditcore.md)|[microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md) collection|Get a list of the [microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md) objects and their properties.|
|[Create auditCoreRoot](../api/security-security-post-auditcore.md)|[microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md)|Create a new [microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md) object.|
|[Get auditCoreRoot](../api/security-auditcoreroot-get.md)|[microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md)|Read the properties and relationships of a [microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md) object.|
|[Update auditCoreRoot](../api/security-auditcoreroot-update.md)|[microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md)|Update the properties of a [microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md) object.|
|[Delete auditCoreRoot](../api/security-security-delete-auditcore.md)|None|Delete a [microsoft.graph.security.auditCoreRoot](../resources/security-auditcoreroot.md) object.|
|[List auditLogQueries](../api/security-auditcoreroot-list-auditlogqueries.md)|[microsoft.graph.security.auditLogQuery](../resources/security-auditlogquery.md) collection|Get the auditLogQuery resources from the auditLogQueries navigation property.|
|[Create auditLogQuery](../api/security-auditcoreroot-post-auditlogqueries.md)|[microsoft.graph.security.auditLogQuery](../resources/security-auditlogquery.md)|Create a new auditLogQuery object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [microsoft.graph.entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|auditLogQueries|[microsoft.graph.security.auditLogQuery](../resources/security-auditlogquery.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.auditCoreRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.auditCoreRoot",
  "id": "String (identifier)"
}
```

