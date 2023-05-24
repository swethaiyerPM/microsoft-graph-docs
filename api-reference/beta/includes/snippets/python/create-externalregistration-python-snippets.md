---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegistrationPostRequestBody()
additional_data = [
'@odata_type' => '#microsoft.graph.externalMeetingRegistration', 
'allowed_registrant' => 'everyone', 
];
request_body.additional_data(additional_data)





await client.me.online_meetings.by_online_meeting_id('onlineMeeting-id').registration.post(request_body = request_body)


```