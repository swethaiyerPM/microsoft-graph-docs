---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Template()
additional_data = [
'id' => 'Slack', 
'application_id' => '{id}', 
'factory_tag' => 'CustomSCIM', 
];
request_body.additional_data(additional_data)




request_configuration = SynchronizationTemplateRequestBuilder.SynchronizationTemplateRequestBuilderPutRequestConfiguration(
headers = {
		'Authorization' : "Bearer <token>",
}

)


await client.applications.by_application_id('application-id').synchronization.templates.by_template_id('synchronizationTemplate-id').put(request_body = request_body, request_configuration = request_configuration)


```