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


requestBody := graphidentity.New$refPatchRequestBody()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Identity().B2xUserFlows().ByB2xUserFlowId("b2xIdentityUserFlow-id").UserFlowIdentityProviders().Ref().Patch(context.Background(), requestBody, nil)


```