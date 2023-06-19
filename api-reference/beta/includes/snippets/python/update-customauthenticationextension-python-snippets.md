---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomAuthenticationExtension()
request_body.@odata_type = '#microsoft.graph.onTokenIssuanceStartCustomExtension'

request_body.display_name = 'onTokenIssuanceStartCustomExtension'

request_body.description = 'Fetch additional claims from custom user store'

endpoint_configuration = CustomExtensionEndpointConfiguration()
endpoint_configuration.@odata_type = '#microsoft.graph.httpRequestEndpoint'

additional_data = [
'target_url' => 'https://authenticationeventsAPI.contoso.com', 
];
endpoint_configuration.additional_data(additional_data)



request_body.endpoint_configuration = endpoint_configuration
authentication_configuration = CustomExtensionAuthenticationConfiguration()
authentication_configuration.@odata_type = '#microsoft.graph.azureAdTokenAuthentication'

additional_data = [
'resource_id' => 'api://authenticationeventsAPI.contoso.com/a13d0fc1-04ab-4ede-b215-63de0174cbb4', 
];
authentication_configuration.additional_data(additional_data)



request_body.authentication_configuration = authentication_configuration
additional_data = [
'claims_for_token_configuration' => claims_for_token_configuration1 = Object()
		claims_for_token_configuration1.claim_id_in_api_response = 'DateOfBirth'


claimsForTokenConfigurationArray []= claimsForTokenConfiguration1;
claims_for_token_configuration2 = Object()
		claims_for_token_configuration2.claim_id_in_api_response = 'CustomRoles'


claimsForTokenConfigurationArray []= claimsForTokenConfiguration2;
request_body.claimsfortokenconfiguration(claimsForTokenConfigurationArray)


];
request_body.additional_data(additional_data)





result = await client.identity.custom_authentication_extensions.by_custom_authentication_extension_id('customAuthenticationExtension-id').patch(request_body = request_body)


```