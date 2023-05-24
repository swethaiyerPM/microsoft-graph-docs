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
	"decision" : "Deny", 
	"justification" : "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.IdentityGovernance().AccessReviews().Definitions().ByDefinitionId("accessReviewScheduleDefinition-id").Instances().ByInstanceId("accessReviewInstance-id").Decisions().ByDecisionId("accessReviewInstanceDecisionItem-id").Post(context.Background(), requestBody, nil)


```