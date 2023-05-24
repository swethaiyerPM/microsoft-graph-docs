---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphcompliance "github.com/microsoftgraph/msgraph-beta-sdk-go/compliance"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphcompliance.NewNoncustodialSource()
additionalData := map[string]interface{}{
	"odataId" : "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Compliance().Ediscovery().Cases().ByCaseId("case-id").SourceCollections().BySourceCollectionId("sourceCollection-id").NoncustodialSources().ByNoncustodialSourceId("noncustodialDataSource-id").Post(context.Background(), requestBody, nil)


```