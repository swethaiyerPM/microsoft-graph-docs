---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.@odata_type = '#microsoft.graph.ipNamedLocation'

request_body.display_name = 'Untrusted IP named location'

additional_data = [
'is_trusted' => false,
'ip_ranges' => ip_ranges1 = Object()
		ip_ranges1.@odata_type = '#microsoft.graph.iPv4CidrRange'

		ip_ranges1.cidr_address = '12.34.221.11/22'


ipRangesArray []= ipRanges1;
ip_ranges2 = Object()
		ip_ranges2.@odata_type = '#microsoft.graph.iPv6CidrRange'

		ip_ranges2.cidr_address = '2001:0:9d38:90d6:0:0:0:0/63'


ipRangesArray []= ipRanges2;
request_body.ipranges(ipRangesArray)


];
request_body.additional_data(additional_data)





result = await client.identity.conditional_access.named_locations.post(request_body = request_body)


```