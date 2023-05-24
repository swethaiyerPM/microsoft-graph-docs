---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeletedItem()
additional_data = [
'user_id' => '55ac777c-109e-4022-b58c-470c8fcb6892', 
'type' => 'Group', 
];
request_body.additional_data(additional_data)





await client.directory.deleted_items.by_deleted_item_id('directoryObject-id').post(request_body = request_body)


```