---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  abstractions "github.com/microsoft/kiota-abstractions-go"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphapplications "github.com/microsoftgraph/msgraph-beta-sdk-go/applications"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


headers := abstractions.NewRequestHeaders()
headers.Add("Authorization", "Bearer <token>")

configuration := &graphapplications.ApplicationItemSynchronizationTemplateItemRequestBuilderPutRequestConfiguration{
	Headers: headers,
}
requestBody := graphapplications.NewTemplate()
additionalData := map[string]interface{}{
	"id" : "Slack", 
	"applicationId" : "{id}", 
	"factoryTag" : "CustomSCIM", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Applications().ByApplicationId("application-id").Synchronization().Templates().ByTemplateId("synchronizationTemplate-id").Put(context.Background(), requestBody, configuration)


```