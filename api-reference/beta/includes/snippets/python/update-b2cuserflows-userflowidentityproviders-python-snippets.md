---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserFlowIdentityProvider()
additional_data = [
'@odata_id' => 'https://graph.microsoft.com/beta/identity/identityProviders/{id}', 
'@odata_type' => '#microsoft.graph.identityProvider', 
];
request_body.additional_data(additional_data)





await client.identity.b2c_user_flows.by_b2c_user_flow_id('b2cIdentityUserFlow-id').user_flow_identity_providers.by_user_flow_identity_provider_id('identityProviderBase-id').patch(request_body = request_body)


```