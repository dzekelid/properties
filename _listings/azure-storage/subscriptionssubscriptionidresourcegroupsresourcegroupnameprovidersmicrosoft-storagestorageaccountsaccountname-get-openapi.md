---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 0
info:
  title: Azure Storage API Storage Accounts Get Properties
  version: 1.0.0
  description: Returns the properties for the specified storage account including
    but not limited to name, SKU name, location, and account status. The ListKeys
    operation should be used to retrieve storage keys.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}:
    get:
      summary: Storage Accounts Get Properties
      description: Returns the properties for the specified storage account including
        but not limited to name, SKU name, location, and account status. The ListKeys
        operation should be used to retrieve storage keys.
      operationId: StorageAccounts_GetProperties
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storagestorageaccountsaccountname-get
      parameters:
      - in: path
        name: accountName
        description: The name of the storage account within the specified resource
          group
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Storage Accounts Properties
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---