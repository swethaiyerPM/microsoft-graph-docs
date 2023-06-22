---
title: "Update userExperienceAnalyticsAnomalyCorrelationGroupOverview"
description: "Update the properties of a userExperienceAnalyticsAnomalyCorrelationGroupOverview object."
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: apiPageType
---

# Update userExperienceAnalyticsAnomalyCorrelationGroupOverview

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Update the properties of a [userExperienceAnalyticsAnomalyCorrelationGroupOverview](../resources/intune-devices-userexperienceanalyticsanomalycorrelationgroupoverview.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAnomalyCorrelationGroupOverview/{userExperienceAnalyticsAnomalyCorrelationGroupOverviewId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsAnomalyCorrelationGroupOverview](../resources/intune-devices-userexperienceanalyticsanomalycorrelationgroupoverview.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsAnomalyCorrelationGroupOverview](../resources/intune-devices-userexperienceanalyticsanomalycorrelationgroupoverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier for the user experience analytics anomaly correlation group overview object.|
|anomalyId|String|The unique identifier of the anomaly. Anomaly details such as name and type can be found in the UserExperienceAnalyticsAnomalySeverityOverview entity.|
|correlationGroupId|String|The unique identifier for the correlation group which will uniquely identify one of the correlation group within an anomaly. The correlation Id can be mapped to the correlation group name by concatinating the correlation group features. Example of correlation group name which is the indicative of concatenated features names are  for names, Contoso manufacture 4.4.1 and Windows 11.22621.1485.|
|correlationGroupFeatures|[userExperienceAnalyticsAnomalyCorrelationGroupFeature](../resources/intune-devices-userexperienceanalyticsanomalycorrelationgroupfeature.md) collection|Describes the features of a device that are shared between all devices in a correlation group.|
|correlationGroupPrevalence|[userExperienceAnalyticsAnomalyCorrelationGroupPrevalence](../resources/intune-devices-userexperienceanalyticsanomalycorrelationgroupprevalence.md)|The prevalence of the correlation group. Possible values are: high, medium or low. Possible values are: `high`, `medium`, `low`, `unknownFutureValue`.|
|correlationGroupPrevalencePercentage|Double|The percentage of the devices in the correlation group that are anomalous. Valid values -1.79769313486232E+308 to 1.79769313486232E+308|
|totalDeviceCount|Int32|Indicates the total number of devices in the tenant. Valid values -2147483648 to 2147483647|
|anomalyCorrelationGroupCount|Int32|Indicates the number of correlation groups in the anomaly. Valid values -2147483648 to 2147483647|
|correlationGroupDeviceCount|Int32|Indicates the total number of devices in a correlation group. Valid values -2147483648 to 2147483647|
|correlationGroupAnomalousDeviceCount|Int32|Indicates the total number of devices affected by the anomaly in the correlation group. Valid values -2147483648 to 2147483647|
|correlationGroupAtRiskDeviceCount|Int32|Indicates the total number of devices at risk in the correlation group. Valid values -2147483648 to 2147483647|



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAnomalyCorrelationGroupOverview](../resources/intune-devices-userexperienceanalyticsanomalycorrelationgroupoverview.md) object in the response body.

## Example

### Request
Here is an example of the request.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAnomalyCorrelationGroupOverview/{userExperienceAnalyticsAnomalyCorrelationGroupOverviewId}
Content-type: application/json
Content-length: 708

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAnomalyCorrelationGroupOverview",
  "anomalyId": "Anomaly Id value",
  "correlationGroupId": "Correlation Group Id value",
  "correlationGroupFeatures": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsAnomalyCorrelationGroupFeature",
      "deviceFeatureType": "model",
      "values": [
        "Values value"
      ]
    }
  ],
  "correlationGroupPrevalence": "medium",
  "correlationGroupPrevalencePercentage": 12.0,
  "totalDeviceCount": 0,
  "anomalyCorrelationGroupCount": 12,
  "correlationGroupDeviceCount": 11,
  "correlationGroupAnomalousDeviceCount": 4,
  "correlationGroupAtRiskDeviceCount": 1
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 757

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAnomalyCorrelationGroupOverview",
  "id": "74f8f469-f469-74f8-69f4-f87469f4f874",
  "anomalyId": "Anomaly Id value",
  "correlationGroupId": "Correlation Group Id value",
  "correlationGroupFeatures": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsAnomalyCorrelationGroupFeature",
      "deviceFeatureType": "model",
      "values": [
        "Values value"
      ]
    }
  ],
  "correlationGroupPrevalence": "medium",
  "correlationGroupPrevalencePercentage": 12.0,
  "totalDeviceCount": 0,
  "anomalyCorrelationGroupCount": 12,
  "correlationGroupDeviceCount": 11,
  "correlationGroupAnomalousDeviceCount": 4,
  "correlationGroupAtRiskDeviceCount": 1
}
```
