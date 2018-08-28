swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/properties:
    get:
      summary: Get a merchant's properties
      description: Get a merchant's properties.
      operationId: GetMerchantProperties
      x-api-path-slug: v3merchantsmidproperties-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Properties
    post:
      summary: Update merchant properties
      description: Update merchant properties.
      operationId: UpdateMerchantProperties
      x-api-path-slug: v3merchantsmidproperties-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Properties