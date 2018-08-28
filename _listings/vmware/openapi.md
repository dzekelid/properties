swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/resources/{resourceId}/properties:
    get:
      summary: Get Properties of a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesPropertiesByResourceIdGet
      x-api-path-slug: apiresourcesresourceidproperties-get
      parameters:
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Properties
    post:
      summary: Add or Update Properties of a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesPropertiesByResourceIdPost
      x-api-path-slug: apiresourcesresourceidproperties-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Properties