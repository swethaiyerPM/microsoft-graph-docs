---
title: "Delete customTaskExtension"
description: "Delete a customTaskExtension object."
author: "AlexFilipin"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# Delete customTaskExtension

Namespace: microsoft.graph.identityGovernance

Delete a [customTaskExtension](../resources/identitygovernance-customtaskextension.md) object. A custom task extension  can only be deleted if it is not referenced in any task objects in a lifecycle workflow.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "identitygovernance_customtaskextension_delete" } -->
[!INCLUDE [permissions-table](../includes/permissions/identitygovernance-customtaskextension-delete-permissions.md)]

[!INCLUDE [rbac-lifecycle-workflows-apis-write](../includes/rbac-for-apis/rbac-lifecycle-workflows-apis-write.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/lifecycleWorkflows/customTaskExtensions/{customTaskExtensionId}/
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "lifecycleworkflows_delete_customtaskextension"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/lifecycleWorkflows/customTaskExtensions/2af4670b-47d3-460f-ad16-fc7d4c511d33
```

### Response

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
