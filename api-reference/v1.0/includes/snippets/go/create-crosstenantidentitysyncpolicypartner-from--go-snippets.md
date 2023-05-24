---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphpolicies "github.com/microsoftgraph/msgraph-sdk-go/policies"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphpolicies.NewIdentitySynchronizationPutRequestBody()
additionalData := map[string]interface{}{
	"displayName" : "Fabrikam", 
userSyncInbound := graphmodels.New()
	isSyncAllowed := true
userSyncInbound.SetIsSyncAllowed(&isSyncAllowed) 
	requestBody.SetUserSyncInbound(userSyncInbound)
}
requestBody.SetAdditionalData(additionalData)

graphClient.Policies().CrossTenantAccessPolicy().Partners().ByPartnerId("crossTenantAccessPolicyConfigurationPartner-tenantId").IdentitySynchronization().Put(context.Background(), requestBody, nil)


```