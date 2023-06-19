---
title: "security resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# security resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get security](../api/security-get.md)|[security](../resources/security.md)|Read the properties and relationships of a [security](../resources/security.md) object.|
|[Update security](../api/security-update.md)|[security](../resources/security.md)|Update the properties of a [security](../resources/security.md) object.|
|[runHuntingQuery](../api/security-runhuntingquery.md)|[huntingQueryResults](../resources/security-huntingqueryresults.md)|**TODO: Add Description**|
|[List alerts](../api/security-security-list-alerts.md)|[alert](../resources/alert.md) collection|Get the alert resources from the alerts navigation property.|
|[Create alert](../api/security-post-alerts.md)|[alert](../resources/alert.md)|Create a new alert object.|
|[List alerts_v2](../api/security-incident-list-alerts.md)|[alert](../resources/security-alert.md) collection|Get the alert resources from the alerts_v2 navigation property.|
|[Create alert](../api/security-post-alerts_v2.md)|[alert](../resources/security-alert.md)|Create a new alert object.|
|[List attackSimulationRoot](../api/security-security-list-attacksimulation.md)|[attackSimulationRoot](../resources/attacksimulationroot.md) collection|Get the attackSimulationRoot resources from the attackSimulation navigation property.|
|[Create attackSimulationRoot](../api/security-post-attacksimulation.md)|[attackSimulationRoot](../resources/attacksimulationroot.md)|Create a new attackSimulationRoot object.|
|[List auditCoreRoot](../api/security-security-list-auditcore.md)|[auditCoreRoot](../resources/security-auditcoreroot.md) collection|Get the auditCoreRoot resources from the auditCore navigation property.|
|[Create auditCoreRoot](../api/security-post-auditcore.md)|[auditCoreRoot](../resources/security-auditcoreroot.md)|Create a new auditCoreRoot object.|
|[List casesRoot](../api/security-security-list-cases.md)|[casesRoot](../resources/security-casesroot.md) collection|Get the casesRoot resources from the cases navigation property.|
|[Create casesRoot](../api/security-post-cases.md)|[casesRoot](../resources/security-casesroot.md)|Create a new casesRoot object.|
|[List cloudAppSecurityProfiles](../api/security-security-list-cloudappsecurityprofiles.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) collection|Get the cloudAppSecurityProfile resources from the cloudAppSecurityProfiles navigation property.|
|[Create cloudAppSecurityProfile](../api/security-post-cloudappsecurityprofiles.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Create a new cloudAppSecurityProfile object.|
|[List domainSecurityProfiles](../api/security-security-list-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md) collection|Get the domainSecurityProfile resources from the domainSecurityProfiles navigation property.|
|[Create domainSecurityProfile](../api/security-post-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Create a new domainSecurityProfile object.|
|[List fileSecurityProfiles](../api/security-security-list-filesecurityprofiles.md)|[fileSecurityProfile](../resources/filesecurityprofile.md) collection|Get the fileSecurityProfile resources from the fileSecurityProfiles navigation property.|
|[Create fileSecurityProfile](../api/security-post-filesecurityprofiles.md)|[fileSecurityProfile](../resources/filesecurityprofile.md)|Create a new fileSecurityProfile object.|
|[List hostSecurityProfiles](../api/security-security-list-hostsecurityprofiles.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md) collection|Get the hostSecurityProfile resources from the hostSecurityProfiles navigation property.|
|[Create hostSecurityProfile](../api/security-post-hostsecurityprofiles.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Create a new hostSecurityProfile object.|
|[List incidents](../api/security-security-list-incidents.md)|[incident](../resources/security-incident.md) collection|Get the incident resources from the incidents navigation property.|
|[Create incident](../api/security-post-incidents.md)|[incident](../resources/security-incident.md)|Create a new incident object.|
|[List informationProtection](../api/security-security-list-informationprotection.md)|[informationProtection](../resources/security-informationprotection.md) collection|Get the informationProtection resources from the informationProtection navigation property.|
|[Create informationProtection](../api/security-post-informationprotection.md)|[informationProtection](../resources/security-informationprotection.md)|Create a new informationProtection object.|
|[List ipSecurityProfiles](../api/security-security-list-ipsecurityprofiles.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md) collection|Get the ipSecurityProfile resources from the ipSecurityProfiles navigation property.|
|[Create ipSecurityProfile](../api/security-post-ipsecurityprofiles.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md)|Create a new ipSecurityProfile object.|
|[List labelsRoot](../api/security-security-list-labels.md)|[labelsRoot](../resources/security-labelsroot.md) collection|Get the labelsRoot resources from the labels navigation property.|
|[Create labelsRoot](../api/security-post-labels.md)|[labelsRoot](../resources/security-labelsroot.md)|Create a new labelsRoot object.|
|[List providerTenantSettings](../api/security-security-list-providertenantsettings.md)|[providerTenantSetting](../resources/providertenantsetting.md) collection|Get the providerTenantSetting resources from the providerTenantSettings navigation property.|
|[Create providerTenantSetting](../api/security-post-providertenantsettings.md)|[providerTenantSetting](../resources/providertenantsetting.md)|Create a new providerTenantSetting object.|
|[List secureScoreControlProfiles](../api/security-security-list-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|Get the secureScoreControlProfile resources from the secureScoreControlProfiles navigation property.|
|[Create secureScoreControlProfile](../api/security-post-securescorecontrolprofiles.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Create a new secureScoreControlProfile object.|
|[List secureScores](../api/security-security-list-securescores.md)|[secureScore](../resources/securescore.md) collection|Get the secureScore resources from the secureScores navigation property.|
|[Create secureScore](../api/security-post-securescores.md)|[secureScore](../resources/securescore.md)|Create a new secureScore object.|
|[List securityActions](../api/security-security-list-securityactions.md)|[securityAction](../resources/securityaction.md) collection|Get the securityAction resources from the securityActions navigation property.|
|[Create securityAction](../api/security-post-securityactions.md)|[securityAction](../resources/securityaction.md)|Create a new securityAction object.|
|[List subjectRightsRequests](../api/privacy-list-subjectrightsrequests.md)|[subjectRightsRequest](../resources/subjectrightsrequest.md) collection|Get the subjectRightsRequest resources from the subjectRightsRequests navigation property.|
|[Create subjectRightsRequest](../api/security-post-subjectrightsrequests.md)|[subjectRightsRequest](../resources/subjectrightsrequest.md)|Create a new subjectRightsRequest object.|
|[List threatIntelligence](../api/security-security-list-threatintelligence.md)|[threatIntelligence](../resources/security-threatintelligence.md) collection|Get the threatIntelligence resources from the threatIntelligence navigation property.|
|[Create threatIntelligence](../api/security-post-threatintelligence.md)|[threatIntelligence](../resources/security-threatintelligence.md)|Create a new threatIntelligence object.|
|[List threatSubmissionRoot](../api/security-security-list-threatsubmission.md)|[threatSubmissionRoot](../resources/security-threatsubmissionroot.md) collection|Get the threatSubmissionRoot resources from the threatSubmission navigation property.|
|[Create threatSubmissionRoot](../api/security-post-threatsubmission.md)|[threatSubmissionRoot](../resources/security-threatsubmissionroot.md)|Create a new threatSubmissionRoot object.|
|[List tiIndicators](../api/security-security-list-tiindicators.md)|[tiIndicator](../resources/tiindicator.md) collection|Get the tiIndicator resources from the tiIndicators navigation property.|
|[Create tiIndicator](../api/security-post-tiindicators.md)|[tiIndicator](../resources/tiindicator.md)|Create a new tiIndicator object.|
|[List triggersRoot](../api/security-security-list-triggers.md)|[triggersRoot](../resources/security-triggersroot.md) collection|Get the triggersRoot resources from the triggers navigation property.|
|[Create triggersRoot](../api/security-post-triggers.md)|[triggersRoot](../resources/security-triggersroot.md)|Create a new triggersRoot object.|
|[List triggerTypesRoot](../api/security-security-list-triggertypes.md)|[triggerTypesRoot](../resources/security-triggertypesroot.md) collection|Get the triggerTypesRoot resources from the triggerTypes navigation property.|
|[Create triggerTypesRoot](../api/security-post-triggertypes.md)|[triggerTypesRoot](../resources/security-triggertypesroot.md)|Create a new triggerTypesRoot object.|
|[List userSecurityProfiles](../api/security-security-list-usersecurityprofiles.md)|[userSecurityProfile](../resources/usersecurityprofile.md) collection|Get the userSecurityProfile resources from the userSecurityProfiles navigation property.|
|[Create userSecurityProfile](../api/security-post-usersecurityprofiles.md)|[userSecurityProfile](../resources/usersecurityprofile.md)|Create a new userSecurityProfile object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|providerStatus|[securityProviderStatus](../resources/securityproviderstatus.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|alerts|[alert](../resources/alert.md) collection|**TODO: Add Description**|
|alerts_v2|[alert](../resources/security-alert.md) collection|**TODO: Add Description**|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|**TODO: Add Description**|
|auditCore|[auditCoreRoot](../resources/security-auditcoreroot.md)|**TODO: Add Description**|
|cases|[casesRoot](../resources/security-casesroot.md)|**TODO: Add Description**|
|cloudAppSecurityProfiles|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) collection|**TODO: Add Description**|
|domainSecurityProfiles|[domainSecurityProfile](../resources/domainsecurityprofile.md) collection|**TODO: Add Description**|
|fileSecurityProfiles|[fileSecurityProfile](../resources/filesecurityprofile.md) collection|**TODO: Add Description**|
|hostSecurityProfiles|[hostSecurityProfile](../resources/hostsecurityprofile.md) collection|**TODO: Add Description**|
|incidents|[incident](../resources/security-incident.md) collection|**TODO: Add Description**|
|informationProtection|[informationProtection](../resources/security-informationprotection.md)|**TODO: Add Description**|
|ipSecurityProfiles|[ipSecurityProfile](../resources/ipsecurityprofile.md) collection|**TODO: Add Description**|
|labels|[labelsRoot](../resources/security-labelsroot.md)|**TODO: Add Description**|
|providerTenantSettings|[providerTenantSetting](../resources/providertenantsetting.md) collection|**TODO: Add Description**|
|secureScoreControlProfiles|[secureScoreControlProfile](../resources/securescorecontrolprofile.md) collection|**TODO: Add Description**|
|secureScores|[secureScore](../resources/securescore.md) collection|**TODO: Add Description**|
|securityActions|[securityAction](../resources/securityaction.md) collection|**TODO: Add Description**|
|subjectRightsRequests|[subjectRightsRequest](../resources/subjectrightsrequest.md) collection|**TODO: Add Description**|
|threatIntelligence|[threatIntelligence](../resources/security-threatintelligence.md)|**TODO: Add Description**|
|threatSubmission|[threatSubmissionRoot](../resources/security-threatsubmissionroot.md)|**TODO: Add Description**|
|tiIndicators|[tiIndicator](../resources/tiindicator.md) collection|**TODO: Add Description**|
|triggers|[triggersRoot](../resources/security-triggersroot.md)|**TODO: Add Description**|
|triggerTypes|[triggerTypesRoot](../resources/security-triggertypesroot.md)|**TODO: Add Description**|
|userSecurityProfiles|[userSecurityProfile](../resources/usersecurityprofile.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security",
  "id": "String (identifier)",
  "providerStatus": [
    {
      "@odata.type": "microsoft.graph.securityProviderStatus"
    }
  ]
}
```

