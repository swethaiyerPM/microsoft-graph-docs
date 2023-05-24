---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphpolicies "github.com/microsoftgraph/msgraph-beta-sdk-go/policies"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphpolicies.NewDeviceRegistrationPolicyPutRequestBody()
additionalData := map[string]interface{}{
	"id" : "deviceRegistrationPolicy", 
	"displayName" : "Device Registration Policy", 
	"description" : "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks", 
	"userDeviceQuota" : int32(50) , 
	"multiFactorAuthConfiguration" : "0", 
azureADRegistration := graphmodels.New()
appliesTo := "1"
azureADRegistration.SetAppliesTo(&appliesTo) 
	isAdminConfigurable := false
azureADRegistration.SetIsAdminConfigurable(&isAdminConfigurable) 
	allowedUsers := []graphmodels.able {

	}
	azureADRegistration.SetAllowedUsers(allowedUsers)
	allowedGroups := []graphmodels.able {

	}
	azureADRegistration.SetAllowedGroups(allowedGroups)
	requestBody.SetAzureADRegistration(azureADRegistration)
azureADJoin := graphmodels.New()
appliesTo := "1"
azureADJoin.SetAppliesTo(&appliesTo) 
	isAdminConfigurable := true
azureADJoin.SetIsAdminConfigurable(&isAdminConfigurable) 
	allowedUsers := []graphmodels.able {

	}
	azureADJoin.SetAllowedUsers(allowedUsers)
	allowedGroups := []graphmodels.able {

	}
	azureADJoin.SetAllowedGroups(allowedGroups)
	requestBody.SetAzureADJoin(azureADJoin)
localAdminPassword := graphmodels.New()
	isEnabled := true
localAdminPassword.SetIsEnabled(&isEnabled) 
	requestBody.SetLocalAdminPassword(localAdminPassword)
}
requestBody.SetAdditionalData(additionalData)

graphClient.Policies().DeviceRegistrationPolicy().Put(context.Background(), requestBody, nil)


```