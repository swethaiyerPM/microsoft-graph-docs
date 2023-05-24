---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RefRequestBuilder.RefRequestBuilderDeleteQueryParameters(
		id = "https://graph.microsoft.com/beta/users/{id}",
)

request_configuration = RefRequestBuilder.RefRequestBuilderDeleteRequestConfiguration(
query_parameters = query_params,
)


await client.groups.by_group_id('group-id').rejected_senders.ref.delete(request_configuration = request_configuration)


```