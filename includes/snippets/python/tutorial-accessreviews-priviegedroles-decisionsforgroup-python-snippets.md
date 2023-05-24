---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Decision()
additional_data = [
'decision' => 'Approve', 
'justification' => 'The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources', 
];
request_body.additional_data(additional_data)





await client.identity_governance.acce_reviews.definitions.by_definition_id('accessReviewScheduleDefinition-id').instances.by_instance_id('accessReviewInstance-id').decisions.by_decision_id('accessReviewInstanceDecisionItem-id').post(request_body = request_body)


```