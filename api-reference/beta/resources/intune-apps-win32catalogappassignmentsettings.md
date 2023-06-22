---
title: "win32CatalogAppAssignmentSettings resource type"
description: "Contains properties used to assign an Win32 catalog mobile app to a group."
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: resourcePageType
---

# win32CatalogAppAssignmentSettings resource type

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Contains properties used to assign an Win32 catalog mobile app to a group.


Inherits from [win32LobAppAssignmentSettings](../resources/intune-shared-win32lobappassignmentsettings.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|notifications|[win32LobAppNotification](../resources/intune-shared-win32lobappnotification.md)|The notification status for this app assignment. Inherited from [win32LobAppAssignmentSettings](../resources/intune-shared-win32lobappassignmentsettings.md). Possible values are: `showAll`, `showReboot`, `hideAll`.|
|restartSettings|[win32LobAppRestartSettings](../resources/intune-shared-win32lobapprestartsettings.md)|The reboot settings to apply for this app assignment. Inherited from [win32LobAppAssignmentSettings](../resources/intune-shared-win32lobappassignmentsettings.md)|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/intune-shared-mobileappinstalltimesettings.md)|The install time settings to apply for this app assignment. Inherited from [win32LobAppAssignmentSettings](../resources/intune-shared-win32lobappassignmentsettings.md)|
|deliveryOptimizationPriority|[win32LobAppDeliveryOptimizationPriority](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|The delivery optimization priority for this app assignment. This setting is not supported in National Cloud environments. Inherited from [win32LobAppAssignmentSettings](../resources/intune-shared-win32lobappassignmentsettings.md). Possible values are: `notConfigured`, `foreground`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32CatalogAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32CatalogAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```
