---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  abstractions "github.com/microsoft/kiota-abstractions-go"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphdevicemanagement "github.com/microsoftgraph/msgraph-beta-sdk-go/devicemanagement"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


headers := abstractions.NewRequestHeaders()
headers.Add("X-MS-CloudPC-USGovCloudTenantAADToken", "{token}")

configuration := &graphdevicemanagement.DeviceManagementVirtualEndpointCrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration{
	Headers: headers,
}
requestBody := graphdevicemanagement.NewCrossCloudGovernmentOrganizationMappingPostRequestBody()

graphClient.DeviceManagement().VirtualEndpoint().CrossCloudGovernmentOrganizationMapping().Post(context.Background(), requestBody, configuration)


```