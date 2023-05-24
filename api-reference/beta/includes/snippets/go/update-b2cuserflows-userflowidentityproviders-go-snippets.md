---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphidentity "github.com/microsoftgraph/msgraph-beta-sdk-go/identity"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphidentity.NewUserFlowIdentityProvider()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/beta/identity/identityProviders/{id}", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Identity().B2cUserFlows().ByB2cUserFlowId("b2cIdentityUserFlow-id").UserFlowIdentityProviders().ByUserFlowIdentityProviderId("identityProviderBase-id").Patch(context.Background(), requestBody, nil)


```