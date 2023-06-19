---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.@odata_type = '#microsoft.graph.educationRubricOutcome'

additional_data = [
'rubric_quality_feedback' => rubric_quality_feedback1 = Object()
		rubric_quality_feedback1.quality_id = '9a145aa8-f3d9-43a1-8f77-5387ff0693f2'

rubric_quality_feedback1feedback = Feedback()
		rubric_quality_feedback1feedback.content = 'This is feedback specific to the first quality of the rubric.'

		rubric_quality_feedback1feedback.content_type = 'text'


rubric_quality_feedback1.feedback = rubric_quality_feedback1feedback

rubricQualityFeedbackArray []= rubricQualityFeedback1;
rubric_quality_feedback2 = Object()
		rubric_quality_feedback2.quality_id = 'd2331fb2-2761-402e-8de6-93e0afaa076e'

rubric_quality_feedback2feedback = Feedback()
		rubric_quality_feedback2feedback.content = 'This is feedback specific to the second quality of the rubric.'

		rubric_quality_feedback2feedback.content_type = 'text'


rubric_quality_feedback2.feedback = rubric_quality_feedback2feedback

rubricQualityFeedbackArray []= rubricQualityFeedback2;
request_body.rubricqualityfeedback(rubricQualityFeedbackArray)


'rubric_quality_selected_levels' => rubric_quality_selected_levels1 = Object()
	rubric_quality_selected_levels1.quality_id = '9a145aa8-f3d9-43a1-8f77-5387ff0693f2'

	rubric_quality_selected_levels1.column_id = '4fb17a1d-5681-46c2-a295-4e305c3eae23'


rubricQualitySelectedLevelsArray []= rubricQualitySelectedLevels1;
rubric_quality_selected_levels2 = Object()
	rubric_quality_selected_levels2.quality_id = 'd2331fb2-2761-402e-8de6-93e0afaa076e'

	rubric_quality_selected_levels2.column_id = 'aac076bf-51ba-48c5-a2e0-ee235b0b9740'


rubricQualitySelectedLevelsArray []= rubricQualitySelectedLevels2;
request_body.rubricqualityselectedlevels(rubricQualitySelectedLevelsArray)


];
request_body.additional_data(additional_data)





result = await client.education.classes.by_classe_id('educationClass-id').assignments.by_assignment_id('educationAssignment-id').submissions.by_submission_id('educationSubmission-id').outcomes.by_outcome_id('educationOutcome-id').patch(request_body = request_body)


```