---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphdirectory "github.com/microsoftgraph/msgraph-sdk-go/directory"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphdirectory.NewDeletedItem()
additionalData := map[string]interface{}{
	"userId" : "55ac777c-109e-4022-b58c-470c8fcb6892", 
	"type" : "Group", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Directory().DeletedItems().ByDeletedItemId("directoryObject-id").Post(context.Background(), requestBody, nil)


```