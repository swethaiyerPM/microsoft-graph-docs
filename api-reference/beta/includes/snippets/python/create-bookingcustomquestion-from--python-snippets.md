---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomQuestion()
additional_data = [
'@odata_type' => '#microsoft.graph.bookingCustomQuestion', 
'display_name' => 'What is your age?', 
'answer_input_type' => 'text', 
'answer_options' => [],
];
request_body.additional_data(additional_data)





await client.booking_businesses.by_booking_businesse_id('bookingBusiness-id').custom_questions.by_custom_question_id('bookingCustomQuestion-id').post(request_body = request_body)


```