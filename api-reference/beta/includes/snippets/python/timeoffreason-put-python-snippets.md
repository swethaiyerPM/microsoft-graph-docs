---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeOffReason()
additional_data = [
'display_name' => 'Vacation', 
'icon_type' => 'plane', 
'is_active' => true,
];
request_body.additional_data(additional_data)




request_configuration = TimeOffReasonRequestBuilder.TimeOffReasonRequestBuilderPutRequestConfiguration(
headers = {
		'Prefer' : "return=representation",
}

)


await client.teams.by_team_id('team-id').schedule.time_off_reasons.by_time_off_reason_id('timeOffReason-id').put(request_body = request_body, request_configuration = request_configuration)


```