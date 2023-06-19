---
title: "Create auditLogQuery"
description: "Create a new microsoft.graph.security.auditLogQuery object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Create auditLogQuery
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [microsoft.graph.security.auditLogQuery](../resources/security-auditlogquery.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/auditCore/auditLogQueries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [microsoft.graph.security.auditLogQuery](../resources/security-auditlogquery.md) object.

You can specify the following properties when creating a **auditLogQuery**.

**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|filterStartDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|filterEndDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|recordTypeFilter|microsoft.graph.security.auditLogRecordType|**TODO: Add Description**. The possible values are: `exchangeAdmin`, `exchangeItem`, `exchangeItemGroup`, `sharePoint`, `syntheticProbe`, `sharePointFileOperation`, `oneDrive`, `azureActiveDirectory`, `azureActiveDirectoryAccountLogon`, `dataCenterSecurityCmdlet`, `complianceDLPSharePoint`, `sway`, `complianceDLPExchange`, `sharePointSharingOperation`, `azureActiveDirectoryStsLogon`, `skypeForBusinessPSTNUsage`, `skypeForBusinessUsersBlocked`, `securityComplianceCenterEOPCmdlet`, `exchangeAggregatedOperation`, `powerBIAudit`, `crm`, `yammer`, `skypeForBusinessCmdlets`, `discovery`, `microsoftTeams`, `threatIntelligence`, `mailSubmission`, `microsoftFlow`, `aeD`, `microsoftStream`, `complianceDLPSharePointClassification`, `threatFinder`, `project`, `sharePointListOperation`, `sharePointCommentOperation`, `dataGovernance`, `kaizala`, `securityComplianceAlerts`, `threatIntelligenceUrl`, `securityComplianceInsights`, `mipLabel`, `workplaceAnalytics`, `powerAppsApp`, `powerAppsPlan`, `threatIntelligenceAtpContent`, `labelContentExplorer`, `teamsHealthcare`, `exchangeItemAggregated`, `hygieneEvent`, `dataInsightsRestApiAudit`, `informationBarrierPolicyApplication`, `sharePointListItemOperation`, `sharePointContentTypeOperation`, `sharePointFieldOperation`, `microsoftTeamsAdmin`, `hrSignal`, `microsoftTeamsDevice`, `microsoftTeamsAnalytics`, `informationWorkerProtection`, `campaign`, `dlpEndpoint`, `airInvestigation`, `quarantine`, `microsoftForms`, `applicationAudit`, `complianceSupervisionExchange`, `customerKeyServiceEncryption`, `officeNative`, `mipAutoLabelSharePointItem`, `mipAutoLabelSharePointPolicyLocation`, `microsoftTeamsShifts`, `secureScore`, `mipAutoLabelExchangeItem`, `cortanaBriefing`, `search`, `wdatpAlerts`, `powerPlatformAdminDlp`, `powerPlatformAdminEnvironment`, `mdatpAudit`, `sensitivityLabelPolicyMatch`, `sensitivityLabelAction`, `sensitivityLabeledFileAction`, `attackSim`, `airManualInvestigation`, `securityComplianceRBAC`, `userTraining`, `airAdminActionInvestigation`, `mstic`, `physicalBadgingSignal`, `teamsEasyApprovals`, `aipDiscover`, `aipSensitivityLabelAction`, `aipProtectionAction`, `aipFileDeleted`, `aipHeartBeat`, `mcasAlerts`, `onPremisesFileShareScannerDlp`, `onPremisesSharePointScannerDlp`, `exchangeSearch`, `sharePointSearch`, `privacyDataMinimization`, `labelAnalyticsAggregate`, `myAnalyticsSettings`, `securityComplianceUserChange`, `complianceDLPExchangeClassification`, `complianceDLPEndpoint`, `mipExactDataMatch`, `msdeResponseActions`, `msdeGeneralSettings`, `msdeIndicatorsSettings`, `ms365DCustomDetection`, `msdeRolesSettings`, `mapgAlerts`, `mapgPolicy`, `mapgRemediation`, `privacyRemediationAction`, `privacyDigestEmail`, `mipAutoLabelSimulationProgress`, `mipAutoLabelSimulationCompletion`, `mipAutoLabelProgressFeedback`, `dlpSensitiveInformationType`, `mipAutoLabelSimulationStatistics`, `largeContentMetadata`, `microsoft365Group`, `cdpMlInferencingResult`, `filteringMailMetadata`, `cdpClassificationMailItem`, `cdpClassificationDocument`, `officeScriptsRunAction`, `filteringPostMailDeliveryAction`, `cdpUnifiedFeedback`, `tenantAllowBlockList`, `consumptionResource`, `healthcareSignal`, `dlpImportResult`, `cdpCompliancePolicyExecution`, `multiStageDisposition`, `privacyDataMatch`, `filteringDocMetadata`, `filteringEmailFeatures`, `powerBIDlp`, `filteringUrlInfo`, `filteringAttachmentInfo`, `coreReportingSettings`, `complianceConnector`, `powerPlatformLockboxResourceAccessRequest`, `powerPlatformLockboxResourceCommand`, `cdpPredictiveCodingLabel`, `cdpCompliancePolicyUserFeedback`, `webpageActivityEndpoint`, `omePortal`, `cmImprovementActionChange`, `filteringUrlClick`, `mipLabelAnalyticsAuditRecord`, `filteringEntityEvent`, `filteringRuleHits`, `filteringMailSubmission`, `labelExplorer`, `microsoftManagedServicePlatform`, `powerPlatformServiceActivity`, `scorePlatformGenericAuditRecord`, `filteringTimeTravelDocMetadata`, `alert`, `alertStatus`, `alertIncident`, `incidentStatus`, `case`, `caseInvestigation`, `recordsManagement`, `privacyRemediation`, `dataShareOperation`, `cdpDlpSensitive`, `ehrConnector`, `filteringMailGradingResult`, `publicFolder`, `privacyTenantAuditHistoryRecord`, `aipScannerDiscoverEvent`, `eduDataLakeDownloadOperation`, `m365ComplianceConnector`, `microsoftGraphDataConnectOperation`, `microsoftPurview`, `filteringEmailContentFeatures`, `powerPagesSite`, `powerAppsResource`, `plannerPlan`, `plannerCopyPlan`, `plannerTask`, `plannerRoster`, `plannerPlanList`, `plannerTaskList`, `plannerTenantSettings`, `projectForTheWebProject`, `projectForTheWebTask`, `projectForTheWebRoadmap`, `projectForTheWebRoadmapItem`, `projectForTheWebProjectSettings`, `projectForTheWebRoadmapSettings`, `quarantineMetadata`, `microsoftTodoAudit`, `timeTravelFilteringDocMetadata`, `teamsQuarantineMetadata`, `sharePointAppPermissionOperation`, `microsoftTeamsSensitivityLabelAction`, `filteringTeamsMetadata`, `filteringTeamsUrlInfo`, `filteringTeamsPostDeliveryAction`, `mdcAssessments`, `mdcRegulatoryComplianceStandards`, `mdcRegulatoryComplianceControls`, `mdcRegulatoryComplianceAssessments`, `mdcSecurityConnectors`, `mdaDataSecuritySignal`, `vivaGoals`, `filteringRuntimeInfo`, `attackSimAdmin`, `microsoftGraphDataConnectConsent`, `filteringAtpDetonationInfo`, `privacyPortal`, `managedTenants`, `unifiedSimulationMatchedItem`, `unifiedSimulationSummary`, `updateQuarantineMetadata`, `ms365DSuppressionRule`, `purviewDataMapOperation`, `filteringUrlPostClickAction`, `irmUserDefinedDetectionSignal`, `teamsUpdates`, `plannerRosterSensitivityLabel`, `ms365DIncident`, `filteringDelistingMetadata`, `complianceDLPSharePointClassificationExtended`, `microsoftDefenderForIdentityAudit`, `supervisoryReviewDayXInsight`, `defenderExpertsforXDRAdmin`, `cdpEdgeBlockedMessage`, `hostedRpa`, `cdpContentExplorerAggregateRecord`, `cdpHygieneAttachmentInfo`, `cdpHygieneSummary`, `cdpPostMailDeliveryAction`, `cdpEmailFeatures`, `cdpHygieneUrlInfo`, `cdpUrlClick`, `cdpPackageManagerHygieneEvent`, `filteringDocScan`, `timeTravelFilteringDocScan`, `mapgOnboard`, `unknownFutureValue`. Optional.|
|keywordFilter|String|**TODO: Add Description** Optional.|
|serviceFilter|String|**TODO: Add Description** Optional.|
|operationFilters|String collection|**TODO: Add Description** Optional.|
|userPrincipalNameFilters|String collection|**TODO: Add Description** Optional.|
|ipAddressFilters|String collection|**TODO: Add Description** Optional.|
|objectIdFilters|String collection|**TODO: Add Description** Optional.|
|administrativeUnitIdFilters|String collection|**TODO: Add Description** Optional.|
|status|microsoft.graph.security.auditLogQueryStatus|**TODO: Add Description**. The possible values are: `notStarted`, `running`, `succeeded`, `failed`, `cancelled`, `unknownFutureValue`. Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [microsoft.graph.security.auditLogQuery](../resources/security-auditlogquery.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_auditlogquery_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/auditCore/auditLogQueries
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.auditLogQuery",
  "displayName": "String",
  "filterStartDateTime": "String (timestamp)",
  "filterEndDateTime": "String (timestamp)",
  "recordTypeFilter": "String",
  "keywordFilter": "String",
  "serviceFilter": "String",
  "operationFilters": [
    "String"
  ],
  "userPrincipalNameFilters": [
    "String"
  ],
  "ipAddressFilters": [
    "String"
  ],
  "objectIdFilters": [
    "String"
  ],
  "administrativeUnitIdFilters": [
    "String"
  ],
  "status": "String"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.auditLogQuery"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.auditLogQuery",
  "id": "168ec429-084b-a489-90d8-504a87846305",
  "displayName": "String",
  "filterStartDateTime": "String (timestamp)",
  "filterEndDateTime": "String (timestamp)",
  "recordTypeFilter": "String",
  "keywordFilter": "String",
  "serviceFilter": "String",
  "operationFilters": [
    "String"
  ],
  "userPrincipalNameFilters": [
    "String"
  ],
  "ipAddressFilters": [
    "String"
  ],
  "objectIdFilters": [
    "String"
  ],
  "administrativeUnitIdFilters": [
    "String"
  ],
  "status": "String"
}
```

