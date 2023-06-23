---
title: "win32MobileAppCatalogPackage resource type"
description: "win32MobileAppCatalogPackage extends mobileAppCatalogPackage by providing information necessary for the creation of a win32CatalogApp instance."
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: resourcePageType
---

# win32MobileAppCatalogPackage resource type

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

win32MobileAppCatalogPackage extends mobileAppCatalogPackage by providing information necessary for the creation of a win32CatalogApp instance.


Inherits from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List win32MobileAppCatalogPackages](../api/intune-apps-win32mobileappcatalogpackage-list.md)|[win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md) collection|List properties and relationships of the [win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md) objects.|
|[Get win32MobileAppCatalogPackage](../api/intune-apps-win32mobileappcatalogpackage-get.md)|[win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md)|Read properties and relationships of the [win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md) object.|
|[Create win32MobileAppCatalogPackage](../api/intune-apps-win32mobileappcatalogpackage-create.md)|[win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md)|Create a new [win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md) object.|
|[Delete win32MobileAppCatalogPackage](../api/intune-apps-win32mobileappcatalogpackage-delete.md)|None|Deletes a [win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md).|
|[Update win32MobileAppCatalogPackage](../api/intune-apps-win32mobileappcatalogpackage-update.md)|[win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md)|Update the properties of a [win32MobileAppCatalogPackage](../resources/intune-apps-win32mobileappcatalogpackage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|icon|[mimeContent](../resources/intune-shared-mimecontent.md)|The icon, if available, to be displayed in the search results. Read-only. Default value is null if no icon is available. Inherited from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|
|id|String|The unique identifier of a specific product, version, and other attributes. Inherited from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|
|productId|String|The identifier of a specific product irrespective of version, or other attributes. Inherited from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|
|productName|String|Name of the product (example: "Fabrikam for Business"). Inherited from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|
|publisher|String|Name of the application catalog package publisher (example: "Fabrikam"). Inherited from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|
|versionName|String|Name of the product version (example: "1.2203.156"). Inherited from [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|
|architectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md) collection|One or more Windows architecture(s) for which this product branch is supported. Possible values are: x86, x64, and arm64.|
|branchId|String|Unique identifier of the branch.|
|branchName|String|The product branch name, which is a specific subset of product functionality as defined by the publisher (example: "Fabrikam for Business (x64)"). A specific product will have one or more branchNames.|
|locales|String collection|One or more locale(s) supported by the branch. Value is a two-letter ISO 639 language tags with optional two-letter subtags (example: en-US, ko, de, de-DE), or mul to indicate multi-language.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32MobileAppCatalogPackage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32MobileAppCatalogPackage",
  "icon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "id": "String (identifier)",
  "productId": "String",
  "productName": "String",
  "publisher": "String",
  "versionName": "String",
  "architectures": [
    "String"
  ],
  "branchId": "String",
  "branchName": "String",
  "locales": [
    "String"
  ]
}
```
