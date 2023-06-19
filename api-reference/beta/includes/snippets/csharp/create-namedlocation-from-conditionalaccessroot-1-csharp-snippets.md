---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NamedLocation
{
	OdataType = "#microsoft.graph.ipNamedLocation",
	DisplayName = "Untrusted IP named location",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"isTrusted" , false
		},
		{
			"ipRanges" , new List<ObjectObject>
			{
				new ObjectObject
				{
					OdataType = "#microsoft.graph.iPv4CidrRange",
					CidrAddress = "12.34.221.11/22",
				},
				new ObjectObject
				{
					OdataType = "#microsoft.graph.iPv6CidrRange",
					CidrAddress = "2001:0:9d38:90d6:0:0:0:0/63",
				},
			}
		},
	},
};
var result = await graphClient.Identity.ConditionalAccess.NamedLocations.PostAsync(requestBody);


```