---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialSource()
additional_data = [
'@odata_id' => 'https://graph.microsoft.com/beta/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339', 
];
request_body.additional_data(additional_data)





await client.security.cases.ediscovery_cases.by_ediscovery_case_id('ediscoveryCase-id').searches.by_searche_id('ediscoverySearch-id').noncustodial_sources.by_noncustodial_source_id('ediscoveryNoncustodialDataSource-id').post(request_body = request_body)


```