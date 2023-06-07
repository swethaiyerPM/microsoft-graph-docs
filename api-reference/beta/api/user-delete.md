---
title: "Delete a user - Microsoft Graph API"
description: "Describes the delete method of the user resource (entity) of the Microsoft Graph API (REST)."
author: "yyuank"
ms.localizationpriority: medium
ms.prod: "users"
doc_type: apiPageType
---

# Delete a user

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete user.  

When deleted, user resources are moved to a temporary container and can be restored within 30 days.  After that time, they are permanently deleted.  To learn more, see [deletedItems](../resources/directory.md).

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadWrite.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.ReadWrite.All |

The calling user must be assigned one of the following Azure AD roles:
+ [User Administrator](/azure/active-directory/roles/permissions-reference#user-administrator)
+ [Privileged Authentication Administrator](/azure/active-directory/roles/permissions-reference#privileged-authentication-administrator)
+ [Global Administrator](/azure/active-directory/roles/permissions-reference#global-administrator)

To delete users with more privileged administrator roles, applications need to be assigned the *Directory.AccessAsUser.All* delegated permission and either the Global Admin role or the Privileged Auth Admin role.

For more details, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference).

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## Request headers

| Header       | Value|
|:-----------|:------|
| Authorization  | Bearer {token}. Required.  |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns `204 No Content` response code. It does not return anything in the response body.

## Example

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```

### Response


The following is an example of the response. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


