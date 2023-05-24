---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphidentitygovernance "github.com/microsoftgraph/msgraph-sdk-go/identitygovernance"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphidentitygovernance.NewDecision()
additionalData := map[string]interface{}{
	"decision" : "Approve", 
	"justification" : "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.IdentityGovernance().AccessReviews().Definitions().ByDefinitionId("accessReviewScheduleDefinition-id").Instances().ByInstanceId("accessReviewInstance-id").Decisions().ByDecisionId("accessReviewInstanceDecisionItem-id").Post(context.Background(), requestBody, nil)


```