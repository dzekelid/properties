---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Get Multi Value Legacy Extended Property
  description: Get multiValueLegacyExtendedProperty Get a resource instance that contains
    a multi-value extended property by using $expand.
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
  /users/{id|userPrincipalName}/messages/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemessagesid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemessagesid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/mailFolders/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemailfoldersid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemailfoldersid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/events/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnameeventsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnameeventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/calendars/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecalendarsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecalendarsid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/contacts/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactsid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactfoldersidcontactsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
  /users/{id|userPrincipalName}/contactFolders/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactfoldersid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactfoldersid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /groups/{id}/threads/{id}/posts/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: groupsidthreadsidpostsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
  /groups/{id}/conversations/{id}/threads/{id}/posts/{id}:
    get:
      summary: Get Multi Value Legacy Extended Property
      description: Get multiValueLegacyExtendedProperty Get a resource instance that
        contains a multi-value extended property by using $expand.
      operationId: GetMultiValueLegacyExtendedProperty
      x-api-path-slug: groupsidconversationsidthreadsidpostsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Value
      - Legacy
      - Extended
      - Property
  /me/messages:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: memessages-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: memessages-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /users/{id|userPrincipalName}/messages:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemessages-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /me/mailFolders:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: memailfolders-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: memailfolders-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /users/{id|userPrincipalName}/mailFolders:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemailfolders-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamemailfolders-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /me/events:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: meevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: meevents-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /users/{id|userPrincipalName}/events:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnameevents-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /me/calendars:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: mecalendars-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: mecalendars-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /users/{id|userPrincipalName}/calendars:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecalendars-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecalendars-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /users/{id|userPrincipalName}/contacts:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontacts-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /me/contactFolders:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: mecontactfolders-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/contactFolders:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactfolders-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactfolders-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /groups/{id}/threads/{id}/posts/{id}/reply:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: groupsidthreadsidpostsidreply-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: groupsidconversationsidthreadsidpostsidreply-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /groups/{id}/threads/{id}/reply:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: groupsidthreadsidreply-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /groups/{id}/conversations/{id}/threads/{id}/reply:
    post:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: groupsidconversationsidthreadsidreply-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /me/contactFolders/{id}:
    patch:
      summary: Create Multi-value Extended Property
      description: Create multi-value extended property Create one or more multi-value
        extended properties in a new or existing instance of a resource.
      operationId: CreateMulti-valueExtendedProperty
      x-api-path-slug: mecontactfoldersid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi-value
      - Extended
      - Property
  /users/{id|userPrincipalName}/contactFolders/{id}/contacts:
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: usersiduserprincipalnamecontactfoldersidcontacts-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: path
        name: id|userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /me/contactfolders:
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: mecontactfolders-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /groups/{id}/threads/{id}/posts:
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: groupsidthreadsidposts-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
  /groups/{id}/conversations/{id}/threads/{id}/posts:
    get:
      summary: Get Single Value Legacy Extended Property
      description: Get singleValueLegacyExtendedProperty Get resource instances that
        contain a single-value extended property by using $expand or $filter.
      operationId: GetSingleValueLegacyExtendedProperty
      x-api-path-slug: groupsidconversationsidthreadsidposts-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Single
      - Value
      - Legacy
      - Extended
      - Property
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