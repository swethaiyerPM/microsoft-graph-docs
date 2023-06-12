---
title: "Delete transcript"
description: "Delete a transcript object."
author: "elmazdremdzhe"
ms.localizationpriority: medium
ms.prod: "sites-and-lists"
doc_type: apiPageType
---

# Delete transcript
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete a [transcript](../resources/transcript.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All |
|Delegated (personal Microsoft account) | Not supported.    |
|Application|Files.ReadWrite.All, Sites.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /drives/{drive-id}/items/{item-id}/media/transcripts/{transcript-id}
DELETE /drives/{drive-id}/root:/{item-path}/media/transcripts/{transcript-id}
DELETE /groups/{group-id}/drive/items/{item-id}/media/transcripts/{transcript-id}
DELETE /groups/{group-id}/drive/root:/{item-path}/media/transcripts/{transcript-id}
DELETE /me/drive/items/{item-id}/media/transcripts/{transcript-id}
DELETE /me/drive/root:/{item-path}/media/transcripts/{transcript-id}
DELETE /sites/{siteId}/drive/items/{itemId}/media/transcripts/{transcript-id}
DELETE /sites/{siteId}/drive/root:/{item-path}/media/transcripts/{transcript-id}
DELETE /users/{userId}/drive/items/{itemId}/media/transcripts/{transcript-id}
DELETE /users/{userId}/drive/root:/{item-path}/media/transcripts/{transcript-id}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|if-match|  If this request header is included and the cTag provided does not match the current tag on the transcript content, a `412 Precondition Failed` response is returned and the transcript will not be deleted. Optional.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

If deleting transcript is still being generated, this method returns a `405 Method Not Allowed` response code.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "delete_transcript"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/drives/1b502de9-89b4-4bba-a44e-a2aab0b4f293/items/01MNC3BE7ZQHKN7ZE67JB2G36IYRIGNWHA/media/transcripts/9415fe71-68b5-42bd-9e5f-86d41ef3efc9
```

### Response
The following is an example of the response
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

