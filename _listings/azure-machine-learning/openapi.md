---
swagger: "2.0"
x-collection-name: Azure Machine Learning
x-complete: 1
info:
  title: Azure ML Web Services Management Client
  description: these-apis-allow-end-users-to-operate-on-azure-machine-learning-web-services-resources--they-support-the-following-operationsullicreate-or-update-a-web-serviceliliget-a-web-servicelilipatch-a-web-servicelilidelete-a-web-serviceliliget-all-web-services-in-a-resource-group-liliget-all-web-services-in-a-subscriptionliliget-web-services-keysliul
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
---