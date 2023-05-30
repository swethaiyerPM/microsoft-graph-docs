---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphappcatalogs "github.com/microsoftgraph/msgraph-sdk-go/appcatalogs"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestRequiresreview := true

requestParameters := &graphappcatalogs.AppCatalogsTeamsAppsRequestBuilderPostQueryParameters{
	Requiresreview: &requestRequiresreview,
}
configuration := &graphappcatalogs.AppCatalogsTeamsAppsRequestBuilderPostRequestConfiguration{
	QueryParameters: requestParameters,
}

graphClient.AppCatalogs().TeamsApps().Post(context.Background(), configuration)


```