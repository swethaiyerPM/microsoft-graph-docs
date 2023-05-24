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


requestBody := graphidentity.NewLanguage()
additionalData := map[string]interface{}{
	"id" : "es-ES", 
	isEnabled := true
requestBody.SetIsEnabled(&isEnabled) 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Identity().B2cUserFlows().ByB2cUserFlowId("b2cIdentityUserFlow-id").Languages().ByLanguageId("userFlowLanguageConfiguration-id").Put(context.Background(), requestBody, nil)


```