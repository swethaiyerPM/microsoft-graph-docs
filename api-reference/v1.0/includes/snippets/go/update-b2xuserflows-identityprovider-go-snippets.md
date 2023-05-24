---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphidentity "github.com/microsoftgraph/msgraph-sdk-go/identity"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphidentity.NewIdentityProvider()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Identity().B2xUserFlows().ByB2xUserFlowId("b2xIdentityUserFlow-id").IdentityProviders().ByIdentityProviderId("identityProvider-id").Post(context.Background(), requestBody, nil)


```