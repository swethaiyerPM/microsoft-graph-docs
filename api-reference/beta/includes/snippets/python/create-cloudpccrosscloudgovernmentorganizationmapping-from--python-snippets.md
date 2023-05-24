---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossCloudGovernmentOrganizationMappingPostRequestBody()


request_configuration = CrossCloudGovernmentOrganizationMappingRequestBuilder.CrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration(
headers = {
		'X-MS-CloudPC-USGovCloudTenantAADToken' : "{token}",
}

)


await client.device_management.virtual_endpoint.cros_cloud_government_organization_mapping.post(request_body = request_body, request_configuration = request_configuration)


```