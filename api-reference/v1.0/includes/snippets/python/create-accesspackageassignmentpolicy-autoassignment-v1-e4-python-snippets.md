---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.display_name = 'A Policy With Questions'

request_body.description = ''

request_body.allowedtargetscope(AllowedTargetScope.AllMemberUsers('allowedtargetscope.allmemberusers'))

expiration = ExpirationPattern()
expiration.type(ExpirationPatternType.NoExpiration('expirationpatterntype.noexpiration'))


request_body.expiration = expiration
requestor_settings = AccessPackageAssignmentRequestorSettings()
requestor_settings.enable_targets_to_self_add_access = True

requestor_settings.enable_targets_to_self_update_access = True

requestor_settings.enable_targets_to_self_remove_access = True


request_body.requestor_settings = requestor_settings
request_approval_settings = AccessPackageAssignmentApprovalSettings()
request_approval_settings.is_approval_required_for_add = True

request_approval_settings.is_approval_required_for_update = True

stages_access_package_approval_stage1 = AccessPackageApprovalStage()
stages_access_package_approval_stage1.durationbeforeautomaticdenial =  \DateInterval('P7D')

stages_access_package_approval_stage1.is_approver_justification_required = False

stages_access_package_approval_stage1.is_escalation_enabled = False

stages_access_package_approval_stage1.FallbackPrimaryApprovers([])

stages_access_package_approval_stage1.EscalationApprovers([])

stages_access_package_approval_stage1.FallbackEscalationApprovers([])

primary_approvers_subject_set1 = SubjectSet()
primary_approvers_subject_set1.@odata_type = '#microsoft.graph.singleUser'

additional_data = [
'user_id' => '08a551cb-575a-4343-b914-f6e42798bd20', 
];
primary_approvers_subject_set1.additional_data(additional_data)



primaryApproversArray []= primaryApproversSubjectSet1;
stages_access_package_approval_stage1.primaryapprovers(primaryApproversArray)



stagesArray []= stagesAccessPackageApprovalStage1;
request_approval_settings.stages(stagesArray)



request_body.request_approval_settings = request_approval_settings
questions_access_package_question1 = AccessPackageQuestion()
questions_access_package_question1.@odata_type = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

questions_access_package_question1.Sequence = 1

questions_access_package_question1.is_required = True

questions_access_package_question1.is_answer_editable = True

questions_access_package_question1.text = 'What country are you working from?'

additional_data = [
'is_multiple_selection_allowed' => 'false', 
'choices' => choices1 = Object()
choices1.@odata_type = 'microsoft.graph.accessPackageAnswerChoice'

choices1.actual_value = 'KE'

choices1.text = 'Kenya'


choicesArray []= choices1;
choices2 = Object()
choices2.@odata_type = 'microsoft.graph.accessPackageAnswerChoice'

choices2.actual_value = 'US'

choices2.text = 'United States'


choicesArray []= choices2;
choices3 = Object()
choices3.@odata_type = 'microsoft.graph.accessPackageAnswerChoice'

choices3.actual_value = 'GY'

choices3.text = 'Guyana'


choicesArray []= choices3;
choices4 = Object()
choices4.@odata_type = 'microsoft.graph.accessPackageAnswerChoice'

choices4.actual_value = 'BD'

choices4.text = 'Bangladesh'


choicesArray []= choices4;
choices5 = Object()
choices5.@odata_type = 'microsoft.graph.accessPackageAnswerChoice'

choices5.actual_value = 'JP'

choices5.text = 'Japan'


choicesArray []= choices5;
questions_access_package_question1.choices(choicesArray)


];
questions_access_package_question1.additional_data(additional_data)



questionsArray []= questionsAccessPackageQuestion1;
questions_access_package_question2 = AccessPackageQuestion()
questions_access_package_question2.@odata_type = '#microsoft.graph.accessPackageTextInputQuestion'

questions_access_package_question2.Sequence = 2

questions_access_package_question2.is_required = True

questions_access_package_question2.is_answer_editable = True

questions_access_package_question2.text = 'What do you do for work?'

localizations_access_package_localized_text1 = AccessPackageLocalizedText()
localizations_access_package_localized_text1.language_code = 'fr-CA'

localizations_access_package_localized_text1.text = 'Que fais-tu comme travail?'


localizationsArray []= localizationsAccessPackageLocalizedText1;
questions_access_package_question2.localizations(localizationsArray)


additional_data = [
'is_single_line_question' => 'false', 
'regex_pattern' => '[a-zA-Z]+[a-zA-Z\s]*', 
];
questions_access_package_question2.additional_data(additional_data)



questionsArray []= questionsAccessPackageQuestion2;
request_body.questions(questionsArray)


access_package = AccessPackage()
access_package.id = '977c7ff4-ef8f-4910-9d31-49048ddf3120'


request_body.access_package = access_package



result = await client.identity_governance.entitlement_management.assignment_policies.post(request_body = request_body)


```