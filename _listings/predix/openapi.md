swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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