---
title: "Get mobileAppCatalogPackage"
description: "Read properties and relationships of the mobileAppCatalogPackage object."
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: apiPageType
---

# Get mobileAppCatalogPackage

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Read properties and relationships of the [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCatalogPackages/{mobileAppCatalogPackageId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.win32CatalogApp/referencedCatalogPackage
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.win32CatalogApp/latestUpgradeCatalogPackage
```

## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md) object in the response body.

## Example

### Request
Here is an example of the request.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCatalogPackages/{mobileAppCatalogPackageId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 428

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCatalogPackage",
    "icon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "id": "3bf2399d-399d-3bf2-9d39-f23b9d39f23b",
    "productId": "Product Id value",
    "productName": "Product Name value",
    "publisher": "Publisher value",
    "versionName": "Version Name value"
  }
}
```
