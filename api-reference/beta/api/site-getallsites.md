---
title: "sites: getAllSites"
description: "List all root sites across geographies in an organization - OneDrive API"
author: tushar20
ms.author: tkanaujia
ms.date: 5/3/2023
ms.localizationpriority: medium
ms.prod: "sharepoint"
doc_type: apiPageType
---

# sites: getAllSites

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

List root [sites](../resources/site.md) across geographies in an organization.

For more details, see [Best practices for discovering files and detecting changes at scale](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online&preserve-view=true).

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "site_getallsites" } -->
[!INCLUDE [permissions-table](../includes/permissions/site-getallsites-permissions.md)]

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /sites/getAllSites
```

## Example

### Request

<!-- { "blockType": "ignored" } -->

```msgraph-interactive
GET /sites/getAllSites
```

### Response

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,bf6fb551-d508-4946-a439-b2a6154fc1d9,65a04b8b-1f44-442b-a1fc-9e5852fb946c",
      "name": "Root Site",
      "root": { },
      "siteCollection": {
        "hostName": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso.sharepoint.com,d9ecf079-9b13-4376-ac5d-f242dda55626,746dbcc1-fa2b-4120-b657-2670bae5bb6f",
      "name": "Site A",
      "root": { },
      "siteCollection": {
        "hostName": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,fd1a778f-263e-4c43-acdf-d5c2519d80eb,c06016db-dfec-4f79-83a1-09c6dbfd7022",
      "name": "Site B",
      "root": { },
      "siteCollection": {
        "hostName": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ],
  "@odata.nextLink": "https://graph.microsoft.com/beta/sites/oneDrive.getAllSites?$skiptoken=U1BHZW9EYXRhTG9jYXRpb25Db2RlYU5BTQ"
}
```
