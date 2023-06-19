---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomerBase()
request_body.@odata_type = '#microsoft.graph.bookingCustomer'

additional_data = [
'display_name' => 'Joni Sherman', 
'email_address' => 'jonis@relecloud.com', 
'addresses' => addresses1 = Object()
		addresses1.post_office_box = ''

		addresses1.street = '4567 Main Street'

		addresses1.city = 'Buffalo'

		addresses1.state = 'NY'

		addresses1.country_or_region = 'USA'

		addresses1.postal_code = '98052'

		addresses1.type = 'home'


addressesArray []= addresses1;
addresses2 = Object()
		addresses2.post_office_box = ''

		addresses2.street = '4570 Main Street'

		addresses2.city = 'Buffalo'

		addresses2.state = 'NY'

		addresses2.country_or_region = 'USA'

		addresses2.postal_code = '98054'

		addresses2.type = 'business'


addressesArray []= addresses2;
request_body.addresses(addressesArray)


'phones' => phones1 = Object()
	phones1.number = '206-555-0100'

	phones1.type = 'home'


phonesArray []= phones1;
phones2 = Object()
	phones2.number = '206-555-0200'

	phones2.type = 'business'


phonesArray []= phones2;
request_body.phones(phonesArray)


];
request_body.additional_data(additional_data)





result = await client.solutions.booking_businesses.by_booking_businesse_id('bookingBusiness-id').customers.post(request_body = request_body)


```