---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SectionGroupsPostRequestBody()
additional_data = [
'display_name' => 'Section group name', 
];
request_body.additional_data(additional_data)





await client.me.onenote.section_groups.by_section_group_id('sectionGroup-id').section_groups.post(request_body = request_body)


```