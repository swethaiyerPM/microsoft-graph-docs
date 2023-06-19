---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewAssignPostRequestBody()
additionalData := map[string]interface{}{


 := graphmodels.NewObject()
id := "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
.SetId(&id) 
target := graphmodels.New()
groupId := "64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
target.SetGroupId(&groupId) 
.SetTarget(target)

	assignments := []graphmodels.Objectable {
		,
	}
}
requestBody.SetAdditionalData(additionalData)

graphClient.DeviceManagement().VirtualEndpoint().ProvisioningPolicies().ByProvisioningPolicieId("cloudPcProvisioningPolicy-id").Assign().Post(context.Background(), requestBody, nil)


```