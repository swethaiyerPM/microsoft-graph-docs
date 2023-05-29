---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphusers "github.com/microsoftgraph/msgraph-sdk-go/users"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestFilter := "Extensions/any"

requestParameters := &graphusers.ItemMessagesRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
	Expand: [] string {"Extensions($filter=id%20eq%20'Com.Contoso.Referral')"},
}
configuration := &graphusers.ItemMessagesRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Me().Messages().Get(context.Background(), configuration)


```