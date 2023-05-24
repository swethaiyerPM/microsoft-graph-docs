---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Column()
additional_data = [
'index' => 3,
];
request_body.additional_data(additional_data)





await client.drives.by_drive_id('drive-id').items.by_item_id('driveItem-id').workbook.tables.by_table_id('workbookTable-id').columns.by_column_id('workbookTableColumn-id').post(request_body = request_body)


```