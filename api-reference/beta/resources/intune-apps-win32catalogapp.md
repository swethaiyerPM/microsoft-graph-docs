---
title: "win32CatalogApp resource type"
description: "A mobileApp that is based on a referenced application in a Win32CatalogApp repository"
author: "jaiprakashmb"
localization_priority: Normal
ms.prod: "intune"
doc_type: resourcePageType
---

# win32CatalogApp resource type

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

A mobileApp that is based on a referenced application in a Win32CatalogApp repository


Inherits from [win32LobApp](../resources/intune-apps-win32lobapp.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List win32CatalogApps](../api/intune-apps-win32catalogapp-list.md)|[win32CatalogApp](../resources/intune-apps-win32catalogapp.md) collection|List properties and relationships of the [win32CatalogApp](../resources/intune-apps-win32catalogapp.md) objects.|
|[Get win32CatalogApp](../api/intune-apps-win32catalogapp-get.md)|[win32CatalogApp](../resources/intune-apps-win32catalogapp.md)|Read properties and relationships of the [win32CatalogApp](../resources/intune-apps-win32catalogapp.md) object.|
|[Create win32CatalogApp](../api/intune-apps-win32catalogapp-create.md)|[win32CatalogApp](../resources/intune-apps-win32catalogapp.md)|Create a new [win32CatalogApp](../resources/intune-apps-win32catalogapp.md) object.|
|[Delete win32CatalogApp](../api/intune-apps-win32catalogapp-delete.md)|None|Deletes a [win32CatalogApp](../resources/intune-apps-win32catalogapp.md).|
|[Update win32CatalogApp](../api/intune-apps-win32catalogapp-update.md)|[win32CatalogApp](../resources/intune-apps-win32catalogapp.md)|Update the properties of a [win32CatalogApp](../resources/intune-apps-win32catalogapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|The upload state. Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersedingAppCount|Int32|The total number of apps this app directly or indirectly supersedes. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersededAppCount|Int32|The total number of apps this app is directly or indirectly superseded by. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|installCommandLine|String|The command line to install this app Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|uninstallCommandLine|String|The command line to uninstall this app Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|The Windows architecture(s) for which this app can run on. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md). Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|The value for the minimum applicable operating system. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|minimumFreeDiskSpaceInMB|Int32|The value for the minimum free disk space which is required to install this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|minimumMemoryInMB|Int32|The value for the minimum physical memory which is required to install this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|minimumNumberOfProcessors|Int32|The value for the minimum number of processors which is required to install this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|minimumCpuSpeedInMHz|Int32|The value for the minimum CPU speed which is required to install this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|detectionRules|[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection|The detection rules to detect Win32 Line of Business (LoB) app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|requirementRules|[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection|The requirement rules to detect Win32 Line of Business (LoB) app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|rules|[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection|The detection and requirement rules for this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|installExperience|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|The install experience for this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|returnCodes|[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection|The return codes for post installation behavior. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|msiInformation|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|The MSI details if this Win32 app is an MSI app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|setupFilePath|String|The relative path of the setup file in the encrypted Win32LobApp package. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|minimumSupportedWindowsRelease|String|The value for the minimum supported windows release. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|displayVersion|String|The version displayed in the UX for this app. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|allowAvailableUninstall|Boolean|When TRUE, indicates that uninstall is supported from the company portal for the Windows app (Win32) with an Available assignment. When FALSE, indicates that uninstall is not supported for the Windows app (Win32) with an Available assignment. Default value is FALSE. Inherited from [win32LobApp](../resources/intune-apps-win32lobapp.md)|
|mobileAppCatalogPackageId|String|The mobileAppCatalogPackageId property references the mobileAppCatalogPackage entity which contains information about an application catalog package that can be deployed to Intune-managed devices|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection|The set of direct relationships for this app. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection|The list of content versions for this app. Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|referencedCatalogPackage|[mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|The current catalog package the app is synced from.|
|latestUpgradeCatalogPackage|[mobileAppCatalogPackage](../resources/intune-apps-mobileappcatalogpackage.md)|The latest available catalog package the app is upgradeable to.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32CatalogApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32CatalogApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "installCommandLine": "String",
  "uninstallCommandLine": "String",
  "applicableArchitectures": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true,
    "v10_2H20": true,
    "v10_21H1": true
  },
  "minimumFreeDiskSpaceInMB": 1024,
  "minimumMemoryInMB": 1024,
  "minimumNumberOfProcessors": 1024,
  "minimumCpuSpeedInMHz": 1024,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String",
      "operator": "String",
      "detectionValue": "String"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "String",
      "detectionValue": "String",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "String",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "operationType": "String",
      "operator": "String",
      "comparisonValue": "String"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "String",
    "deviceRestartBehavior": "String"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 1024,
      "type": "String"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "String",
    "productVersion": "String",
    "upgradeCode": "String",
    "requiresReboot": true,
    "packageType": "String",
    "productName": "String",
    "publisher": "String"
  },
  "setupFilePath": "String",
  "minimumSupportedWindowsRelease": "String",
  "displayVersion": "String",
  "allowAvailableUninstall": true,
  "mobileAppCatalogPackageId": "String"
}
```
