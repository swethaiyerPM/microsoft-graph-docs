---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphdrives "github.com/microsoftgraph/msgraph-beta-sdk-go/drives"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphdrives.NewColumn()
additionalData := map[string]interface{}{
index := graphmodels.New()
	requestBody.SetIndex(index)
}
requestBody.SetAdditionalData(additionalData)

graphClient.Drives().ByDriveId("drive-id").Items().ByItemId("driveItem-id").Workbook().Tables().ByTableId("workbookTable-id").Columns().ByColumnId("workbookTableColumn-id").Post(context.Background(), requestBody, nil)


```