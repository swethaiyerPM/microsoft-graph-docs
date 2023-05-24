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


requestBody := graphusers.NewSectionGroupsPostRequestBody()
additionalData := map[string]interface{}{
	"displayName" : "Section group name", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Me().Onenote().SectionGroups().BySectionGroupId("sectionGroup-id").SectionGroups().Post(context.Background(), requestBody, nil)


```