---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphadministrativeunits "github.com/microsoftgraph/msgraph-beta-sdk-go/administrativeunits"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphadministrativeunits.NewMembersPostRequestBody()
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

graphClient.AdministrativeUnits().ByAdministrativeUnitId("administrativeUnit-id").Members().Post(context.Background(), requestBody, nil)


```