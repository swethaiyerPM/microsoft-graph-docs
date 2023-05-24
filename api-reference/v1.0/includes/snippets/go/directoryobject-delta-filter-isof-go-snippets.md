---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphdirectoryobjects "github.com/microsoftgraph/msgraph-sdk-go/directoryobjects"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestFilter := "isof or isof"

requestParameters := &graphdirectoryobjects.DirectoryObjectsDelta()RequestBuilderGetQueryParameters{
	Filter: &requestFilter,
}
configuration := &graphdirectoryobjects.DirectoryObjectsDelta()RequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.DirectoryObjects().Delta().Get(context.Background(), configuration)


```