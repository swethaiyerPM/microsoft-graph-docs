---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MembersPostRequestBody()
additional_data = [
'@odata_type' => '#microsoft.graph.group', 
'description' => 'Self help community for golf', 
'display_name' => 'Golf Assist', 
'group_types' => ['Unified', ],
'mail_enabled' => true,
'mail_nickname' => 'golfassist', 
'security_enabled' => false,
];
request_body.additional_data(additional_data)





await client.directory.administrative_units.by_administrative_unit_id('administrativeUnit-id').members.post(request_body = request_body)


```