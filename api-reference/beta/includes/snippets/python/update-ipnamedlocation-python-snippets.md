---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.@odata_type = '#microsoft.graph.ipNamedLocation'

request_body.display_name = 'Untrusted named location with only IPv4 address'

additional_data = [
'is_trusted' => false,
'ip_ranges' => ip_ranges1 = Object()
		ip_ranges1.@odata_type = '#microsoft.graph.iPv4CidrRange'

		ip_ranges1.cidr_address = '6.5.4.3/18'


ipRangesArray []= ipRanges1;
request_body.ipranges(ipRangesArray)


];
request_body.additional_data(additional_data)





result = await client.identity.conditional_access.named_locations.by_named_location_id('namedLocation-id').patch(request_body = request_body)


```