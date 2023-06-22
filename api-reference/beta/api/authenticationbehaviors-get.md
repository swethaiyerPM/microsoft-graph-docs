---
title: "Get authenticationBehavior"
description: "Get a single authentication behavior"
author: "medhir"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Get authenticationBehavior

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieves the value of a single authentication behavior from the [authenticationBehaviors](../resources/authenticationbehaviors.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see `[Permissions](/graph/permissions-reference)`.

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)     | Application.ReadWrite.All|
|Delegated (personal Microsoft account) | Application.ReadWrite.All |
|Application    | Application.ReadWrite.OwnedBy, Application.ReadWrite.All  |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{applicationObjectId}/authenticationBehaviors/{authenticationBehavior}
```

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |
| Content-Type  | application/json. Reqiured. 

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a single authentication behavior from the [authenticationBehaviors](../resources/authenticationbehaviors.md) object in the response body.

## Examples

### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "get_authenticationBehavior"
}-->

```http
GET /applications(appId='{appId}')/authenticationBehaviors/removeUnverifiedEmailClaim
```

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.authenticationBehaviors.removeUnverifiedEmailClaim"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications('{appId}')/authenticationBehaviors/removeUnverifiedEmailClaim",
    "value": true
}
```
