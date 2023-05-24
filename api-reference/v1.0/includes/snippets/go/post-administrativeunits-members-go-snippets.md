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


requestBody := graphdirectory.NewMembersPostRequestBody()
additionalData := map[string]interface{}{
	"description" : "Self help community for golf", 
	"displayName" : "Golf Assist", 
	groupTypes := []string {
		"Unified",

	}
	mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled) 
	"mailNickname" : "golfassist", 
	securityEnabled := false
requestBody.SetSecurityEnabled(&securityEnabled) 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Directory().AdministrativeUnits().ByAdministrativeUnitId("administrativeUnit-id").Members().Post(context.Background(), requestBody, nil)


```