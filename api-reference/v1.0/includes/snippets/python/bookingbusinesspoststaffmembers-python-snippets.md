---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingStaffMemberBase()
request_body.@odata_type = '#microsoft.graph.bookingStaffMember'

additional_data = [
'display_name' => 'Dana Swope', 
'email_address' => 'danas@contoso.com', 
'role@odata_type' => '#microsoft.graph.bookingStaffRole', 
'role' => 'externalGuest', 
'time_zone' => 'America/Chicago', 
'use_business_hours' => true,
'working_hours@odata_type' => '#Collection(microsoft.graph.bookingWorkHours)', 
'working_hours' => working_hours1 = Object()
		working_hours1.@odata_type = '#microsoft.graph.bookingWorkHours'

		working_hours1.day@odata_type = '#microsoft.graph.dayOfWeek'

		working_hours1.day = 'monday'

		working_hours1.time_slots@odata_type = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

time_slots1 = Object()
		time_slots1.@odata_type = '#microsoft.graph.bookingWorkTimeSlot'

		time_slots1.end_time = '17:00:00.0000000'

		time_slots1.start_time = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
working_hours1.timeslots(timeSlotsArray)



workingHoursArray []= workingHours1;
working_hours2 = Object()
	working_hours2.@odata_type = '#microsoft.graph.bookingWorkHours'

	working_hours2.day@odata_type = '#microsoft.graph.dayOfWeek'

	working_hours2.day = 'tuesday'

	working_hours2.time_slots@odata_type = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

time_slots1 = Object()
	time_slots1.@odata_type = '#microsoft.graph.bookingWorkTimeSlot'

	time_slots1.end_time = '17:00:00.0000000'

	time_slots1.start_time = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
working_hours2.timeslots(timeSlotsArray)



workingHoursArray []= workingHours2;
working_hours3 = Object()
working_hours3.@odata_type = '#microsoft.graph.bookingWorkHours'

working_hours3.day@odata_type = '#microsoft.graph.dayOfWeek'

working_hours3.day = 'wednesday'

working_hours3.time_slots@odata_type = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

time_slots1 = Object()
time_slots1.@odata_type = '#microsoft.graph.bookingWorkTimeSlot'

time_slots1.end_time = '17:00:00.0000000'

time_slots1.start_time = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
working_hours3.timeslots(timeSlotsArray)



workingHoursArray []= workingHours3;
working_hours4 = Object()
working_hours4.@odata_type = '#microsoft.graph.bookingWorkHours'

working_hours4.day@odata_type = '#microsoft.graph.dayOfWeek'

working_hours4.day = 'thursday'

working_hours4.time_slots@odata_type = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

time_slots1 = Object()
time_slots1.@odata_type = '#microsoft.graph.bookingWorkTimeSlot'

time_slots1.end_time = '17:00:00.0000000'

time_slots1.start_time = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
working_hours4.timeslots(timeSlotsArray)



workingHoursArray []= workingHours4;
working_hours5 = Object()
working_hours5.@odata_type = '#microsoft.graph.bookingWorkHours'

working_hours5.day@odata_type = '#microsoft.graph.dayOfWeek'

working_hours5.day = 'friday'

working_hours5.time_slots@odata_type = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

time_slots1 = Object()
time_slots1.@odata_type = '#microsoft.graph.bookingWorkTimeSlot'

time_slots1.end_time = '17:00:00.0000000'

time_slots1.start_time = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
working_hours5.timeslots(timeSlotsArray)



workingHoursArray []= workingHours5;
request_body.workinghours(workingHoursArray)


'is_email_notification_enabled' => false,
];
request_body.additional_data(additional_data)





result = await client.solutions.booking_businesses.by_booking_businesse_id('bookingBusiness-id').staff_members.post(request_body = request_body)


```