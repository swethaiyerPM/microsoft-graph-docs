---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TeamsRequestBuilder.TeamsRequestBuilderGetQueryParameters(
		filter = "startswith(displayName,%20'A')",
		top = 2,
)

request_configuration = TeamsRequestBuilder.TeamsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


await client.teams.get(request_configuration = request_configuration)


```