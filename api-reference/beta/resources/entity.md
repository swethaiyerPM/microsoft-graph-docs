---
title: "entity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# entity resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List entities](../api/trending-list-resource.md)|[entity](../resources/entity.md) collection|Get a list of the [entity](../resources/entity.md) objects and their properties.|
|[Create entity](../api/trending-post-resource.md)|[entity](../resources/entity.md)|Create a new [entity](../resources/entity.md) object.|
|[Get entity](../api/entity-get.md)|[entity](../resources/entity.md)|Read the properties and relationships of an [entity](../resources/entity.md) object.|
|[Update entity](../api/entity-update.md)|[entity](../resources/entity.md)|Update the properties of an [entity](../resources/entity.md) object.|
|[Delete entity](../api/trending-delete-resource.md)|None|Delete an [entity](../resources/entity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entity",
  "id": "String (identifier)"
}
```

