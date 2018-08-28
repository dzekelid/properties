---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get space properties
  description: "Returns all properties for the given space. Space properties are a
    key-value storage associated with a space.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
    \u2018View\u2019 permission for the space."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{id}/child/attachment/{attachmentId}:
    put:
      summary: Update attachment properties
      description: "Updates the attachment properties, i.e. the non-binary data of
        an attachment \nlike the filename, media-type, comment, and parent container.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.AttachmentResource.updateAttachmentProperties_put
      x-api-path-slug: contentidchildattachmentattachmentid-put
      parameters:
      - in: path
        name: attachmentId
        description: The ID of the attachment to update
      - in: path
        name: id
        description: The ID of the content that the attachment is attached to
      responses:
        200:
          description: OK
      tags:
      - Attachment
      - Properties
  /content/{id}/property:
    get:
      summary: Get content properties
      description: "Returns the properties for a piece of content. For more information
        \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'View' permission for the space, and permission to view the
        content if it is a page."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentPropertyResource.getContentProperties_get
      x-api-path-slug: contentidproperty-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the content
          to expand
      - in: path
        name: id
        description: The ID of the content to be queried for its properties
      - in: query
        name: limit
        description: The maximum number of properties to return per page
      - in: query
        name: start
        description: The starting index of the returned properties
      responses:
        200:
          description: OK
      tags:
      - Content
      - Properties
  /space/{spaceKey}/property:
    get:
      summary: Get space properties
      description: "Returns all properties for the given space. Space properties are
        a key-value storage associated with a space.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
        \u2018View\u2019 permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpacePropertyResource.getSpaceProperties_get
      x-api-path-slug: spacespacekeyproperty-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the spaceproperty
          to expand
      - in: query
        name: limit
        description: The maximum number of properties to return per page
      - in: path
        name: spaceKey
        description: The key of the space to be queried for its properties
      - in: query
        name: start
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Space
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