---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/items/{item-id}:
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: medriveitemsitemid-patch
      parameters:
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /me/drive/root:/{item-path}:
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: medriverootitempath-patch
      parameters:
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /drives/{drive-id}/items/{item-id}:
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: drivesdriveiditemsitemid-patch
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
  /groups/{group-id}/drive/items/{item-id}:
    patch:
      summary: Update Drive Item Properties
      description: Update DriveItem properties Update the metadata for a DriveItem
        by ID or path.
      operationId: UpdateDriveItemProperties
      x-api-path-slug: groupsgroupiddriveitemsitemid-patch
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current eTag on the folder, a 412 Precondition Failed
          response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Properties
---