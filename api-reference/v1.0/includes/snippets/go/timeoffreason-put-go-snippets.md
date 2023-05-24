---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  abstractions "github.com/microsoft/kiota-abstractions-go"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphteams "github.com/microsoftgraph/msgraph-sdk-go/teams"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


headers := abstractions.NewRequestHeaders()
headers.Add("Prefer", "return=representation")

configuration := &graphteams.TeamItemScheduleTimeOffReasonItemRequestBuilderPutRequestConfiguration{
	Headers: headers,
}
requestBody := graphteams.NewTimeOffReason()
additionalData := map[string]interface{}{
	"displayName" : "Vacation", 
	"iconType" : "plane", 
	isActive := true
requestBody.SetIsActive(&isActive) 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Teams().ByTeamId("team-id").Schedule().TimeOffReasons().ByTimeOffReasonId("timeOffReason-id").Put(context.Background(), requestBody, configuration)


```