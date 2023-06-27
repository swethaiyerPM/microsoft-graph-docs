---
title: "Create identitySynchronization"
description: "Create a cross-tenant user synchronization policy for a partner-specific configuration."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Create identitySynchronization

Namespace: microsoft.graph

Create a cross-tenant user synchronization policy for a partner-specific configuration.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "crosstenantaccesspolicyconfigurationpartner_put_identitysynchronization" } -->
[!INCLUDE [permissions-table](../includes/permissions/crosstenantaccesspolicyconfigurationpartner-put-identitysynchronization-permissions.md)]

The signed-in user must also be assigned the following minimum [directory role](/azure/active-directory/roles/permissions-reference):

* Security Administrator

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/crossTenantAccessPolicy/partners/{id}/identitySynchronization
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [crossTenantIdentitySyncPolicyPartner](../resources/crosstenantidentitysyncpolicypartner.md) object.

You can specify the following properties when you create a **crossTenantIdentitySyncPolicyPartner**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name for the cross-tenant user synchronization policy. Use the name of the partner Azure Active Directory tenant to easily identify the policy. Optional.|
|userSyncInbound|[crossTenantUserSyncInbound](../resources/crosstenantusersyncinbound.md)|Determines whether users are synchronized from the partner tenant.|

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following is an example of a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_crosstenantidentitysyncpolicypartner_from_"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/partners/90e29127-71ad-49c7-9ce8-db3f41ea06f1/identitySynchronization
Content-Type: application/json

{
  "displayName": "Fabrikam",
  "userSyncInbound": {
    "isSyncAllowed": true
  }
}
```

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-crosstenantidentitysyncpolicypartner-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-crosstenantidentitysyncpolicypartner-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
