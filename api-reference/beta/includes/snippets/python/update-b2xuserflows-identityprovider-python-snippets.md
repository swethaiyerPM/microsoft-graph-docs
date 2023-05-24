---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
additional_data = [
'@odata_id' => 'https://graph.microsoft.com/beta/identityProviders/{id}', 
];
request_body.additional_data(additional_data)





await client.identity.b2x_user_flows.by_b2x_user_flow_id('b2xIdentityUserFlow-id').identity_providers.by_identity_provider_id('identityProvider-id').post(request_body = request_body)


```