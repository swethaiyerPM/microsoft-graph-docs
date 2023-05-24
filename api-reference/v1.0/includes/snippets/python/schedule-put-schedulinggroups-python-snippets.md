---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchedulingGroup()
additional_data = [
'display_name' => 'Cashiers', 
'is_active' => true,
'user_ids' => ['c5d0c76b-80c4-481c-be50-923cd8d680a1', '2a4296b3-a28a-44ba-bc66-0274b9b95851', ],
];
request_body.additional_data(additional_data)




request_configuration = SchedulingGroupRequestBuilder.SchedulingGroupRequestBuilderPutRequestConfiguration(
headers = {
	'Prefer' : "return=representation",
}

)


await client.teams.by_team_id('team-id').schedule.scheduling_groups.by_scheduling_group_id('schedulingGroup-id').put(request_body = request_body, request_configuration = request_configuration)


```