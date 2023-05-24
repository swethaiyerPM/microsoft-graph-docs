---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AppManagementPolicie()
additional_data = [
'@odata_id' => 'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}', 
];
request_body.additional_data(additional_data)





await client.service_principals.by_service_principal_id('servicePrincipal-id').app_management_policies.by_app_management_policie_id('appManagementPolicy-id').post(request_body = request_body)


```