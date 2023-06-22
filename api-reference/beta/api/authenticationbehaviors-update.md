---
title: "Update authenticationBehaviors"
description: "Update the collection of authentication behaviors"
author: "medhir"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Update authenticationBehaviors

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the collection of [authenticationBehaviors](../resources/authenticationbehaviors.md). Updating can be used to either set, un-set, or update the value of authentication behaviors in the context of an application.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)     | Application.ReadWrite.All|
|Delegated (personal Microsoft account) | Application.ReadWrite.All |
|Application    | Application.ReadWrite.OwnedBy, Application.ReadWrite.All  |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
PATCH /applications/{applicationObjectId}/authenticationBehaviors
```

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |
| Content-Type  | application/json. Reqiured. 

## Request body

In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, don't include existing values that haven't changed.

|Property|Type|Description|
|:---|:---|:---|
|removeUnverifiedEmailClaim|Boolean| Removes the `email` claim from tokens sent to an application when the email address's domain cannot be verified. |

## Response

If successful, this method returns a `200 OK` response code and a single [authenticationBehaviors](../resources/authenticationbehaviors.md)  object in the response body.


## Examples

### Example 1: Set the value of a previously unset authentication behavior

This operation adds a behavior (from a set of valid, pre-defined behaviors) in order to explictly opt-in to the new authentication behavior.

#### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "update_authenticationBehaviors"
}-->

```http
PATCH /applications(appId='{appId}')/authenticationBehaviors
Content-Type: application/json

{
    "removeUnverifiedEmailClaim": true
}
```

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 No Content
```

### Example 2: Re-set the value of a previously set authentication behavior

This operation changes the value of a behavior from a previously set value.

#### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "update_authenticationBehaviors"
}-->

```http
PATCH /applications(appId='{appId}')/authenticationBehaviors
Content-Type: application/json

{
    "removeUnverifiedEmailClaim": false
}
```

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 No Content
```


### Example 3: Unset an authentication behavior for an application

This operation removes the previoulsy set value for a behavior in the context of an application.

#### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "update_authenticationBehaviors"
}-->

```http
PATCH /applications(appId='{appId}')/authenticationBehaviors
Content-Type: application/json

{
    "removeUnverifiedEmailClaim": null
}
```

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 No Content
```
