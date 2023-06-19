---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.access_package_id = 'b2eba9a1-b357-42ee-83a8-336522ed6cbf'

request_body.display_name = 'Users from connected organizations can request'

request_body.description = 'Allow users from configured connected organizations to request and be approved by their sponsors'

request_body.can_extend = False

request_body.DurationInDays = 365

request_body.expirationDateTime=null

requestor_settings = RequestorSettings()
requestor_settings.scope_type = 'AllExistingConnectedOrganizationSubjects'

requestor_settings.accept_requests = True


request_body.requestor_settings = requestor_settings
request_approval_settings = ApprovalSettings()
request_approval_settings.is_approval_required = True

request_approval_settings.is_approval_required_for_extension = False

request_approval_settings.is_requestor_justification_required = True

request_approval_settings.approval_mode = 'SingleStage'

approval_stages_approval_stage1 = ApprovalStage()
approval_stages_approval_stage1.ApprovalStageTimeOutInDays = 14

approval_stages_approval_stage1.is_approver_justification_required = True

approval_stages_approval_stage1.is_escalation_enabled = False

approval_stages_approval_stage1.EscalationTimeInMinutes = 11520

primary_approvers_user_set1 = UserSet()
primary_approvers_user_set1.@odata_type = '#microsoft.graph.groupMembers'

primary_approvers_user_set1.is_backup = True

additional_data = [
'id' => 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primary_approvers_user_set1.additional_data(additional_data)



primaryApproversArray []= primaryApproversUserSet1;
primary_approvers_user_set2 = UserSet()
primary_approvers_user_set2.@odata_type = '#microsoft.graph.externalSponsors'

primary_approvers_user_set2.is_backup = False


primaryApproversArray []= primaryApproversUserSet2;
approval_stages_approval_stage1.primaryapprovers(primaryApproversArray)



approvalStagesArray []= approvalStagesApprovalStage1;
request_approval_settings.approvalstages(approvalStagesArray)



request_body.request_approval_settings = request_approval_settings
questions_access_package_question1 = AccessPackageQuestion()
questions_access_package_question1.is_required = False

questions_access_package_question1text = AccessPackageLocalizedContent()
questions_access_package_question1text.default_text = 'what state are you from?'

localized_texts_access_package_localized_text1 = AccessPackageLocalizedText()
localized_texts_access_package_localized_text1.text = '¿De qué estado eres?'

localized_texts_access_package_localized_text1.language_code = 'es'


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questions_access_package_question1text.localizedtexts(localizedTextsArray)



questions_access_package_question1.text = questions_access_package_question1text
questions_access_package_question1.@odata_type = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

additional_data = [
'choices' => choices1 = Object()
choices1.actual_value = 'AZ'

choices1display_value = DisplayValue()
localized_texts1 = Object()
localized_texts1.text = 'Arizona'

localized_texts1.language_code = 'es'


localizedTextsArray []= localizedTexts1;
choices1display_value.localizedtexts(localizedTextsArray)



choices1.display_value = choices1display_value

choicesArray []= choices1;
choices2 = Object()
choices2.actual_value = 'CA'

choices2display_value = DisplayValue()
localized_texts1 = Object()
localized_texts1.text = 'California'

localized_texts1.language_code = 'es'


localizedTextsArray []= localizedTexts1;
choices2display_value.localizedtexts(localizedTextsArray)



choices2.display_value = choices2display_value

choicesArray []= choices2;
choices3 = Object()
choices3.actual_value = 'OH'

choices3display_value = DisplayValue()
localized_texts1 = Object()
localized_texts1.text = 'Ohio'

localized_texts1.language_code = 'es'


localizedTextsArray []= localizedTexts1;
choices3display_value.localizedtexts(localizedTextsArray)



choices3.display_value = choices3display_value

choicesArray []= choices3;
questions_access_package_question1.choices(choicesArray)


'allows_multiple_selection' => false,
];
questions_access_package_question1.additional_data(additional_data)



questionsArray []= questionsAccessPackageQuestion1;
questions_access_package_question2 = AccessPackageQuestion()
questions_access_package_question2.is_required = False

questions_access_package_question2text = AccessPackageLocalizedContent()
questions_access_package_question2text.default_text = 'Who is your manager?'

localized_texts_access_package_localized_text1 = AccessPackageLocalizedText()
localized_texts_access_package_localized_text1.text = 'por qué necesita acceso a este paquete'

localized_texts_access_package_localized_text1.language_code = 'es'


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questions_access_package_question2text.localizedtexts(localizedTextsArray)



questions_access_package_question2.text = questions_access_package_question2text
questions_access_package_question2.@odata_type = '#microsoft.graph.accessPackageTextInputQuestion'

additional_data = [
'is_single_line_question' => false,
];
questions_access_package_question2.additional_data(additional_data)



questionsArray []= questionsAccessPackageQuestion2;
request_body.questions(questionsArray)





result = await client.identity_governance.entitlement_management.acces_package_assignment_policies.post(request_body = request_body)


```