---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialSource()
additional_data = [
'@odata_id' => 'https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246', 
];
request_body.additional_data(additional_data)





await client.compliance.ediscovery.cases.by_case_id('case-id').source_collections.by_source_collection_id('sourceCollection-id').noncustodial_sources.by_noncustodial_source_id('noncustodialDataSource-id').post(request_body = request_body)


```