---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphbookingbusinesses "github.com/microsoftgraph/msgraph-beta-sdk-go/bookingbusinesses"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphbookingbusinesses.NewCustomQuestion()
additionalData := map[string]interface{}{
	"displayName" : "What is your age?", 
	"answerInputType" : "text", 
	answerOptions := []graphmodels.able {

	}
}
requestBody.SetAdditionalData(additionalData)

graphClient.BookingBusinesses().ByBookingBusinesseId("bookingBusiness-id").CustomQuestions().ByCustomQuestionId("bookingCustomQuestion-id").Post(context.Background(), requestBody, nil)


```