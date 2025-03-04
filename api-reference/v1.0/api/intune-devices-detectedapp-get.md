---
title: "Get detectedApp"
description: "Read properties and relationships of the detectedApp object."
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: apiPageType
---

# Get detectedApp

Namespace: microsoft.graph

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
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
If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.

## Example

### Request
Here is an example of the request.

<!-- { "blockType": "request" , "name" : "intune_devices_detectedapp_get_get_detectedapp" }-->
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

<!-- { "blockType": "response" , "@odata.type" : "microsoft.graph.detectedApp" }-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 312

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11,
    "publisher": "Publisher value",
    "platform": "windows"
  }
}
```
