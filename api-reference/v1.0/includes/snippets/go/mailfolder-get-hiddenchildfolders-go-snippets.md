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



requestIncludehiddenfolders := true

requestParameters := &graphusers.ItemMailFolderItemChildFoldersRequestBuilderGetQueryParameters{
	Includehiddenfolders: &requestIncludehiddenfolders,
}
configuration := &graphusers.ItemMailFolderItemChildFoldersRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Me().MailFolders().ByMailFolderId("mailFolder-id").ChildFolders().Get(context.Background(), configuration)


```