---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Intelligent Mapping Update the layer properties
  description: |-
    For the layer identified by the specified map and layer identifiers,
    updates the layer properties.
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/system/audit/changes:
    get:
      summary: Get property-level audit records.
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAuditChanges
      x-api-path-slug: v1systemauditchanges-get
      parameters:
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      responses:
        200:
          description: Successful response
      tags:
      - Property-level
      - Audit
      - Records
  /v1/maps/{mapId}/layers/{layerId}:
    put:
      summary: Update the layer properties
      description: |-
        For the layer identified by the specified map and layer identifiers,
        updates the layer properties.
      operationId: for-the-layer-identified-by-the-specified-map-and-layer-identifiersupdates-the-layer-properties
      x-api-path-slug: v1mapsmapidlayerslayerid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Layer
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