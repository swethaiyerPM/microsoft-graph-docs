---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AnswerPostRequestBody()
request_body.callback_uri = 'https://bot.contoso.com/api/calls'

request_body.AcceptedModalities([request_body.modality(Modality.Audio('modality.audio'))
])

media_config = MediaConfig()
media_config.@odata_type = '#microsoft.graph.serviceHostedMediaConfig'

additional_data = [
'pre_fetch_media' => pre_fetch_media1 = Object()
	pre_fetch_media1.uri = 'https://cdn.contoso.com/beep.wav'

	pre_fetch_media1.resource_id = '1D6DE2D4-CD51-4309-8DAA-70768651088E'


preFetchMediaArray []= preFetchMedia1;
pre_fetch_media2 = Object()
	pre_fetch_media2.uri = 'https://cdn.contoso.com/cool.wav'

	pre_fetch_media2.resource_id = '1D6DE2D4-CD51-4309-8DAA-70768651088F'


preFetchMediaArray []= preFetchMedia2;
media_config.prefetchmedia(preFetchMediaArray)


];
media_config.additional_data(additional_data)



request_body.media_config = media_config



await client.communications.calls.by_call_id('call-id').answer.post(request_body = request_body)


```