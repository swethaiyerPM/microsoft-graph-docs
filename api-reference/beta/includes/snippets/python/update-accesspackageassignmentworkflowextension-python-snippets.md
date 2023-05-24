---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageCustomWorkflowExtension()
additional_data = [
'@odata_type' => '#microsoft.graph.accessPackageAssignmentWorkflowExtension', 
'display_name' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
request_body.additional_data(additional_data)





await client.identity_governance.entitlement_management.acce_package_catalogs.by_acce_package_catalog_id('accessPackageCatalog-id').acce_package_custom_workflow_extensions.by_acces_package_custom_workflow_extension_id('customCalloutExtension-id').put(request_body = request_body)


```