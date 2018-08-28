---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Delete content property
  description: "Deletes a content property. For more information about content properties,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
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
    post:
      summary: Create content property
      description: "Creates a property for an existing piece of content. For more
        information \nabout content properties, see [Content properties in the REST
        API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
        is the same as [Create content property for key](#api-content-id-property-key-post)
        \nexcept that the key is specified in the request body instead of as a \npath
        parameter.\n\nContent properties can also be added when creating a new piece
        of content \nby including them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentPropertyResource.createContentProperty_pos
      x-api-path-slug: contentidproperty-post
      parameters:
      - in: path
        name: id
        description: The ID of the content to add the property to
      responses:
        200:
          description: OK
      tags:
      - Content
      - Property
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
    post:
      summary: Create space property
      description: "Creates a new space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
        permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpacePropertyResource.createSpaceProperty_post
      x-api-path-slug: spacespacekeyproperty-post
      parameters:
      - in: path
        name: spaceKey
        description: The key of the space that the property will be created in
      responses:
        200:
          description: OK
      tags:
      - Space
      - Property
  /content/{id}/property/{key}:
    get:
      summary: Get content property
      description: "Returns a content property for a piece of content. For more information,
        see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'View' permission for the space, and permission to view the
        content if it is a page."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentPropertyResource.getContentProperty_get
      x-api-path-slug: contentidpropertykey-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the content
          to expand
      - in: path
        name: id
        description: The ID of the content to be queried for the property
      - in: path
        name: key
        description: The key of the content property
      responses:
        200:
          description: OK
      tags:
      - Content
      - Property
    put:
      summary: Update content property
      description: "Updates an existing content property. This method will also create
        a new \nproperty for a piece of content, if the property key does not exist
        and \nthe property version is 1. For more information about content properties,
        see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentPropertyResource.updateContentProperty_put
      x-api-path-slug: contentidpropertykey-put
      parameters:
      - in: path
        name: id
        description: The ID of the content that the property belongs to
      - in: path
        name: key
        description: The key of the property
      responses:
        200:
          description: OK
      tags:
      - Content
      - Property
    delete:
      summary: Delete content property
      description: "Deletes a content property. For more information about content
        properties, see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentPropertyResource.deleteContentProperty_del
      x-api-path-slug: contentidpropertykey-delete
      parameters:
      - in: path
        name: id
        description: The ID of the content that the property belongs to
      - in: path
        name: key
        description: The key of the property
      responses:
        200:
          description: OK
      tags:
      - Content
      - Property
    post:
      summary: Create content property for key
      description: "Creates a property for an existing piece of content. For more
        information \nabout content properties, see [Content properties in the REST
        API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
        is the same as [Create content property](#api-content-id-property-post) \nexcept
        that the key is specified as a path parameter instead of in the \nrequest
        body.\n\nContent properties can also be added when creating a new piece of
        content \nby including them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentPropertyResource.createContentPropertyForK
      x-api-path-slug: contentidpropertykey-post
      parameters:
      - in: path
        name: id
        description: The ID of the content to add the property to
      - in: path
        name: key
        description: The key of the content property
      responses:
        200:
          description: OK
      tags:
      - Content
      - Propertykey
  /space/{spaceKey}/property/{key}:
    get:
      summary: Get space property
      description: "Returns a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
        \u2018View\u2019 permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpacePropertyResource.getSpaceProperty_get
      x-api-path-slug: spacespacekeypropertykey-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the spaceproperty
          to expand
      - in: path
        name: key
        description: The key of the space property
      - in: path
        name: spaceKey
        description: The key of the space that the property is in
      responses:
        200:
          description: OK
      tags:
      - Space
      - Property
    put:
      summary: Update space property
      description: "Updates a space property. Note, you cannot update the key of a
        space\nproperty, only the value.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
        permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpacePropertyResource.updateSpaceProperty_put
      x-api-path-slug: spacespacekeypropertykey-put
      parameters:
      - in: path
        name: key
        description: The key of the property to be updated
      - in: path
        name: spaceKey
        description: The key of the space that the property is in
      responses:
        200:
          description: OK
      tags:
      - Space
      - Property
    delete:
      summary: Delete space property
      description: "Deletes a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
        permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpacePropertyResource.deleteSpaceProperty_delete
      x-api-path-slug: spacespacekeypropertykey-delete
      parameters:
      - in: path
        name: key
        description: The key of the property to be deleted
      - in: path
        name: spaceKey
        description: The key of the space that the property is in
      responses:
        200:
          description: OK
      tags:
      - Space
      - Property
    post:
      summary: Create space property for key
      description: "Creates a new space property. This is the same as `POST\n/space/{spaceKey}/property`
        but the key for the property is passed as a\npath parameter, rather than in
        the request body.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
        permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpacePropertyResource.createSpacePropertyForKey_p
      x-api-path-slug: spacespacekeypropertykey-post
      parameters:
      - in: path
        name: key
        description: The key of the property to be created
      - in: path
        name: spaceKey
        description: The key of the space that the property will be created in
      responses:
        200:
          description: OK
      tags:
      - Space
      - Propertykey
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