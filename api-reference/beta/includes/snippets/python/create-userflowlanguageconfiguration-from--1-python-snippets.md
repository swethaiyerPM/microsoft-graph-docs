---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Language()
additional_data = [
'id' => 'es-ES', 
'is_enabled' => true,
];
request_body.additional_data(additional_data)





await client.identity.b2c_user_flows.by_b2c_user_flow_id('b2cIdentityUserFlow-id').languages.by_language_id('userFlowLanguageConfiguration-id').put(request_body = request_body)


```