---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Me().Activities().ByActivitieId("userActivity-id").HistoryItems().ByHistoryItemId("activityHistoryItem-id").Put(context.Background(), nil)


```