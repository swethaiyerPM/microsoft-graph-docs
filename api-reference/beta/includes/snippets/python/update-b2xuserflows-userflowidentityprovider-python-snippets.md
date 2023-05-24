---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $RefPatchRequestBody()
additional_data = [
'@odata_id' => 'https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test', 
'@odata_type' => '#microsoft.graph.identityProvider', 
];
request_body.additional_data(additional_data)





await client.identity.b2x_user_flows.by_b2x_user_flow_id('b2xIdentityUserFlow-id').user_flow_identity_providers.ref.patch(request_body = request_body)


```