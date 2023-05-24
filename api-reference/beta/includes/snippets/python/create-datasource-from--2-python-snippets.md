---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustodianSource()
additional_data = [
'@odata_id' => 'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531', 
];
request_body.additional_data(additional_data)





await client.compliance.ediscovery.cases.by_case_id('case-id').source_collections.by_source_collection_id('sourceCollection-id').custodian_sources.by_custodian_source_id('dataSource-id').post(request_body = request_body)


```