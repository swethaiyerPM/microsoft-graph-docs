---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphusers "github.com/microsoftgraph/msgraph-beta-sdk-go/users"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphusers.NewRegistrationPostRequestBody()
additionalData := map[string]interface{}{
	"allowedRegistrant" : "everyone", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Me().OnlineMeetings().ByOnlineMeetingId("onlineMeeting-id").Registration().Post(context.Background(), requestBody, nil)


```