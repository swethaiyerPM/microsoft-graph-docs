---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MeetingRegistrantBase()
request_body.@odata_type = '#microsoft.graph.meetingRegistrant'

additional_data = [
'first_name' => 'Frederick', 
'last_name' => 'Cormier', 
'email' => 'frederick.cormier@contoso.com', 
'custom_question_answers' => custom_question_answers1 = Object()
		custom_question_answers1.question_id = 'MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU='

		custom_question_answers1.value = 'No'


customQuestionAnswersArray []= customQuestionAnswers1;
custom_question_answers2 = Object()
		custom_question_answers2.question_id = 'MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8='

		custom_question_answers2.value = 'Internet'


customQuestionAnswersArray []= customQuestionAnswers2;
request_body.customquestionanswers(customQuestionAnswersArray)


];
request_body.additional_data(additional_data)





result = await client.users.by_user_id('user-id').online_meetings.by_online_meeting_id('onlineMeeting-id').registration.registrants.post(request_body = request_body)


```