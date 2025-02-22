---
title: "Delete community"
description: "Delete a community in Viva Engage."
author: "aditijha4"
ms.localizationpriority: medium
ms.subservice: "viva-engage"
doc_type: apiPageType
---

# Delete community

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete a Viva Engage [community](../resources/community.md) along with all associated Microsoft 365 content, including the connected Microsoft 365 group, OneNote notebook, and Planner plans. For more information, see [What happens if I delete a Viva Engage community connected to Microsoft 365 groups](/viva/engage/engage-microsoft-365-groups#q-what-happens-if-i-delete-a-viva-engage-community-connected-to-microsoft-365-groups).

[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- {
  "blockType": "permissions",
  "name": "community-delete-permissions"
}
-->
[!INCLUDE [permissions-table](../includes/permissions/community-delete-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /employeeExperience/communities/{communityId}
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body

Don't supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "delete_community",
  "sampleKeys": ["eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI4MzIxMjc1In0"]
}
-->
``` http
DELETE https://graph.microsoft.com/beta/employeeExperience/communities/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI4MzIxMjc1In0
```

### Response

The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

