---
title: "mobileAppCatalogPackage resource type"
description: "mobileAppCatalogPackage is an abstract type that application catalog package entities derive from. A mobileAppCatalogPackage entity contains information about an application catalog package that can be deployed to Intune-managed devices."
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: resourcePageType
---

# mobileAppCatalogPackage resource type

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

mobileAppCatalogPackage is an abstract type that application catalog package entities derive from. A mobileAppCatalogPackage entity contains information about an application catalog package that can be deployed to Intune-managed devices.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppCatalogPackage](../api/intune-apps-mobileappcatalogpackage-get.md)|[mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|Read properties and relationships of the [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md) object.|
|[getVariants function](../api/intune-apps-mobileappcatalogpackage-getvariants.md)|[mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md) collection|Not yet documented|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|icon|[mimeContent](../resources/intune-shared-mimecontent.md)|The icon, if available, to be displayed in the search results. Read-only. Default value is null if no icon is available.|
|id|String|The unique identifier of a specific product, version, and other attributes.|
|productId|String|The identifier of a specific product irrespective of version, or other attributes.|
|productName|String|Name of the product (example: "Fabrikam for Business").|
|publisher|String|Name of the application catalog package publisher (example: "Fabrikam").|
|versionName|String|Name of the product version (example: "1.2203.156").|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCatalogPackage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCatalogPackage",
  "icon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "id": "String (identifier)",
  "productId": "String",
  "productName": "String",
  "publisher": "String",
  "versionName": "String"
}
```
