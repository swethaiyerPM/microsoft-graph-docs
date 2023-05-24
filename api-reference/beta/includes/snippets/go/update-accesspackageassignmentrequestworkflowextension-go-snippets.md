---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphidentitygovernance "github.com/microsoftgraph/msgraph-beta-sdk-go/identitygovernance"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphidentitygovernance.NewAccessPackageCustomWorkflowExtension()
additionalData := map[string]interface{}{
	"displayName" : "test_action_0124_email", 
	"description" : "this is for graph testing only", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogs().ByAccessPackageCatalogId("accessPackageCatalog-id").AccessPackageCustomWorkflowExtensions().ByAccessPackageCustomWorkflowExtensionId("customCalloutExtension-id").Put(context.Background(), requestBody, nil)


```