---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 0
info:
  title: Azure API Management API Properties ListByService
  description: Lists a collection of properties defined within a service instance.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/properties
  : get:
      summary: Properties ListByService
      description: Lists a collection of properties defined within a service instance.
      operationId: Properties_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameproperties-get
      parameters:
      - in: query
        name: $filter
        description: '| Field | Supported operators    | Supported functions                                   ||-------|------------------------|-------------------------------------------------------||
          tags  | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith,
          any, all || name  | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith           |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Properties
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