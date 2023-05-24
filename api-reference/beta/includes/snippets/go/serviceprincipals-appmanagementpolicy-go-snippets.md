---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphserviceprincipals "github.com/microsoftgraph/msgraph-beta-sdk-go/serviceprincipals"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphserviceprincipals.NewAppManagementPolicie()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.ServicePrincipals().ByServicePrincipalId("servicePrincipal-id").AppManagementPolicies().ByAppManagementPolicieId("appManagementPolicy-id").Post(context.Background(), requestBody, nil)


```