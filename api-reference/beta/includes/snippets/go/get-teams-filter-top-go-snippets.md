---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphteams "github.com/microsoftgraph/msgraph-beta-sdk-go/teams"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestFilter := "startswith(displayName,%20'A')"
requestTop := int32(2)

requestParameters := &graphteams.TeamsRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
	Top: &requestTop,
}
configuration := &graphteams.TeamsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

graphClient.Teams().Get(context.Background(), configuration)


```