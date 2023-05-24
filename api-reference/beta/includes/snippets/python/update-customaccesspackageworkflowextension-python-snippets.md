---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomAccessPackageWorkflowExtension()
additional_data = [
'@odata_type' => '#microsoft.graph.customAccessPackageWorkflowExtension', 
'display_name' => 'test_action_0124_email', 
'description' => 'this is for graph testing only', 
];
request_body.additional_data(additional_data)





await client.identity_governance.entitlement_management.acce_package_catalogs.by_acce_package_catalog_id('accessPackageCatalog-id').custom_acce_package_workflow_extensions.by_custom_acces_package_workflow_extension_id('customAccessPackageWorkflowExtension-id').put(request_body = request_body)


```