---
swagger: "2.0"
x-collection-name: Azure Machine Learning
x-complete: 0
info:
  title: Azure Machine Learning API Web Services Create Regional Properties
  description: Creates an encrypted credentials parameter blob for the specified region.
    To get the web service from a region other than the region in which it has been
    created, you must first call Create Regional Web Services Properties to create
    a copy of the encrypted credential parameter blob in that region. You only need
    to do this before the first time that you get the web service in the new region.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearning/webServices/{webServiceName}/CreateRegionalBlob
  : post:
      summary: Web Services Create Regional Properties
      description: Creates an encrypted credentials parameter blob for the specified
        region. To get the web service from a region other than the region in which
        it has been created, you must first call Create Regional Web Services Properties
        to create a copy of the encrypted credential parameter blob in that region.
        You only need to do this before the first time that you get the web service
        in the new region.
      operationId: WebServices_CreateRegionalProperties
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-machinelearningwebserviceswebservicenamecreateregionalblob-post
      parameters:
      - in: query
        name: No Name
      - in: query
        name: region
        description: The region for which encrypted credential parameters are created
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Web Services Regional Properties
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