---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphsecurity "github.com/microsoftgraph/msgraph-sdk-go/security"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphsecurity.NewCustodianSource()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/c25c3914-f9f7-43ee-9cba-a25377e0cec6", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Security().Cases().EdiscoveryCases().ByEdiscoveryCaseId("ediscoveryCase-id").Searches().BySearcheId("ediscoverySearch-id").CustodianSources().ByCustodianSourceId("dataSource-id").Post(context.Background(), requestBody, nil)


```