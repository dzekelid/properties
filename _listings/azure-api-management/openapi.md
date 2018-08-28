swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 1
info:
  title: ApiManagementClient
  description: use-these-rest-apis-for-performing-operations-on-user-entity-in-azure-api-management-deployment--the-user-entity-in-api-management-represents-the-developers-that-call-the-apis-of-the-products-to-which-they-are-subscribed-
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/properties/{propId}
  : get:
      summary: Property Get
      description: Gets the details of the property specified by its identifier.
      operationId: Property_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamepropertiespropid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Properties
    put:
      summary: Property CreateOrUpdate
      description: Creates or updates a property.
      operationId: Property_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamepropertiespropid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Properties
    patch:
      summary: Property Update
      description: Updates the specific property.
      operationId: Property_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamepropertiespropid-patch
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the property to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Properties
    delete:
      summary: Property Delete
      description: Deletes specific property from the the API Management service instance.
      operationId: Property_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamepropertiespropid-delete
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the property to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Properties