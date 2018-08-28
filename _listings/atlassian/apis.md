---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Properties
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Update attachment properties
  x-api-slug: contentidchildattachmentattachmentid-put
  description: "Updates the attachment properties, i.e. the non-binary data of an
    attachment \nlike the filename, media-type, comment, and parent container.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidchildattachmentattachmentid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidchildattachmentattachmentid-put-openapi.md
- name: The Confluence Cloud REST API - Get content properties
  x-api-slug: contentidproperty-get
  description: "Returns the properties for a piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'View' permission for the space, and permission to view the content
    if it is a page."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-get-openapi.md
- name: The Confluence Cloud REST API - Get space properties
  x-api-slug: spacespacekeyproperty-get
  description: "Returns all properties for the given space. Space properties are a
    key-value storage associated with a space.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
    \u2018View\u2019 permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-get-openapi.md
- name: The Confluence Cloud REST API - Create content property
  x-api-slug: contentidproperty-post
  description: "Creates a property for an existing piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
    is the same as [Create content property for key](#api-content-id-property-key-post)
    \nexcept that the key is specified in the request body instead of as a \npath
    parameter.\n\nContent properties can also be added when creating a new piece of
    content \nby including them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-post-openapi.md
- name: The Confluence Cloud REST API - Get content property
  x-api-slug: contentidpropertykey-get
  description: "Returns a content property for a piece of content. For more information,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'View' permission for the space, and permission to view the content
    if it is a page."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Update content property
  x-api-slug: contentidpropertykey-put
  description: "Updates an existing content property. This method will also create
    a new \nproperty for a piece of content, if the property key does not exist and
    \nthe property version is 1. For more information about content properties, see
    \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Delete content property
  x-api-slug: contentidpropertykey-delete
  description: "Deletes a content property. For more information about content properties,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Create space property
  x-api-slug: spacespacekeyproperty-post
  description: "Creates a new space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-openapi.md
- name: The Confluence Cloud REST API - Get space property
  x-api-slug: spacespacekeypropertykey-get
  description: "Returns a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
    \u2018View\u2019 permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Update space property
  x-api-slug: spacespacekeypropertykey-put
  description: "Updates a space property. Note, you cannot update the key of a space\nproperty,
    only the value.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Delete space property
  x-api-slug: spacespacekeypropertykey-delete
  description: "Deletes a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Create content property for key
  x-api-slug: contentidpropertykey-post
  description: "Creates a property for an existing piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
    is the same as [Create content property](#api-content-id-property-post) \nexcept
    that the key is specified as a path parameter instead of in the \nrequest body.\n\nContent
    properties can also be added when creating a new piece of content \nby including
    them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-post-openapi.md
- name: The Confluence Cloud REST API - Create space property for key
  x-api-slug: spacespacekeypropertykey-post
  description: "Creates a new space property. This is the same as `POST\n/space/{spaceKey}/property`
    but the key for the property is passed as a\npath parameter, rather than in the
    request body.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-openapi.md
- name: The Confluence Cloud REST API - Create content property
  x-api-slug: contentidproperty-post
  description: "Creates a property for an existing piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
    is the same as [Create content property for key](#api-content-id-property-key-post)
    \nexcept that the key is specified in the request body instead of as a \npath
    parameter.\n\nContent properties can also be added when creating a new piece of
    content \nby including them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-post-openapi.md
- name: The Confluence Cloud REST API - Get content property
  x-api-slug: contentidpropertykey-get
  description: "Returns a content property for a piece of content. For more information,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'View' permission for the space, and permission to view the content
    if it is a page."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Update content property
  x-api-slug: contentidpropertykey-put
  description: "Updates an existing content property. This method will also create
    a new \nproperty for a piece of content, if the property key does not exist and
    \nthe property version is 1. For more information about content properties, see
    \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Delete content property
  x-api-slug: contentidpropertykey-delete
  description: "Deletes a content property. For more information about content properties,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Create space property
  x-api-slug: spacespacekeyproperty-post
  description: "Creates a new space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-openapi.md
- name: The Confluence Cloud REST API - Get space property
  x-api-slug: spacespacekeypropertykey-get
  description: "Returns a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
    \u2018View\u2019 permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Update space property
  x-api-slug: spacespacekeypropertykey-put
  description: "Updates a space property. Note, you cannot update the key of a space\nproperty,
    only the value.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Delete space property
  x-api-slug: spacespacekeypropertykey-delete
  description: "Deletes a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Create content property for key
  x-api-slug: contentidpropertykey-post
  description: "Creates a property for an existing piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
    is the same as [Create content property](#api-content-id-property-post) \nexcept
    that the key is specified as a path parameter instead of in the \nrequest body.\n\nContent
    properties can also be added when creating a new piece of content \nby including
    them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-post-openapi.md
- name: The Confluence Cloud REST API - Create space property for key
  x-api-slug: spacespacekeypropertykey-post
  description: "Creates a new space property. This is the same as `POST\n/space/{spaceKey}/property`
    but the key for the property is passed as a\npath parameter, rather than in the
    request body.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-openapi.md
- name: The Confluence Cloud REST API - Delete space property
  x-api-slug: spacespacekeypropertykey-delete
  description: "Deletes a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Delete space property
  x-api-slug: spacespacekeypropertykey-delete
  description: "Deletes a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Update space property
  x-api-slug: spacespacekeypropertykey-put
  description: "Updates a space property. Note, you cannot update the key of a space\nproperty,
    only the value.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Update space property
  x-api-slug: spacespacekeypropertykey-put
  description: "Updates a space property. Note, you cannot update the key of a space\nproperty,
    only the value.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Get space property
  x-api-slug: spacespacekeypropertykey-get
  description: "Returns a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
    \u2018View\u2019 permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Get space property
  x-api-slug: spacespacekeypropertykey-get
  description: "Returns a space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:
    \u2018View\u2019 permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Create space property
  x-api-slug: spacespacekeyproperty-post
  description: "Creates a new space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-openapi.md
- name: The Confluence Cloud REST API - Create space property
  x-api-slug: spacespacekeyproperty-post
  description: "Creates a new space property.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeyproperty-post-openapi.md
- name: The Confluence Cloud REST API - Delete content property
  x-api-slug: contentidpropertykey-delete
  description: "Deletes a content property. For more information about content properties,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-delete-openapi.md
- name: The Confluence Cloud REST API - Update content property
  x-api-slug: contentidpropertykey-put
  description: "Updates an existing content property. This method will also create
    a new \nproperty for a piece of content, if the property key does not exist and
    \nthe property version is 1. For more information about content properties, see
    \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Update content property
  x-api-slug: contentidpropertykey-put
  description: "Updates an existing content property. This method will also create
    a new \nproperty for a piece of content, if the property key does not exist and
    \nthe property version is 1. For more information about content properties, see
    \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-put-openapi.md
- name: The Confluence Cloud REST API - Get content property
  x-api-slug: contentidpropertykey-get
  description: "Returns a content property for a piece of content. For more information,
    see \n[Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'View' permission for the space, and permission to view the content
    if it is a page."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-get-openapi.md
- name: The Confluence Cloud REST API - Create content property
  x-api-slug: contentidproperty-post
  description: "Creates a property for an existing piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
    is the same as [Create content property for key](#api-content-id-property-key-post)
    \nexcept that the key is specified in the request body instead of as a \npath
    parameter.\n\nContent properties can also be added when creating a new piece of
    content \nby including them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidproperty-post-openapi.md
- name: The Confluence Cloud REST API - Create space property for key
  x-api-slug: spacespacekeypropertykey-post
  description: "Creates a new space property. This is the same as `POST\n/space/{spaceKey}/property`
    but the key for the property is passed as a\npath parameter, rather than in the
    request body.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-openapi.md
- name: The Confluence Cloud REST API - Create space property for key
  x-api-slug: spacespacekeypropertykey-post
  description: "Creates a new space property. This is the same as `POST\n/space/{spaceKey}/property`
    but the key for the property is passed as a\npath parameter, rather than in the
    request body.\n\n**[Permissions required](https://confluence.atlassian.com/x/_AozKw)**:\n\u2018Admin\u2019
    permission for the space."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/spacespacekeypropertykey-post-openapi.md
- name: The Confluence Cloud REST API - Create content property for key
  x-api-slug: contentidpropertykey-post
  description: "Creates a property for an existing piece of content. For more information
    \nabout content properties, see [Content properties in the REST API](https://developer.atlassian.com/cloud/confluence/content-properties/).\n\nThis
    is the same as [Create content property](#api-content-id-property-post) \nexcept
    that the key is specified as a path parameter instead of in the \nrequest body.\n\nContent
    properties can also be added when creating a new piece of content \nby including
    them in the `metadata.properties` of the request.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/contentidpropertykey-post-openapi.md
- name: Jira Cloud REST API - Get workflow transition properties
  x-api-slug: api2workflowtransitionstransitionidproperties-get
  description: |-
    Returns the properties on a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-get-openapi.md
- name: Jira Cloud REST API - Get application property
  x-api-slug: api2applicationproperties-get
  description: Returns an application property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-openapi.md
- name: Jira Cloud REST API - Set application property
  x-api-slug: api2applicationpropertiesid-put
  description: Modify an application property via PUT. The "value" field present in
    the PUT will override the existing value.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-openapi.md
- name: Jira Cloud REST API - Get comment property keys
  x-api-slug: api2commentcommentidproperties-get
  description: Returns the keys of all properties for the comment identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-openapi.md
- name: Jira Cloud REST API - Get comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the comment
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-put
  description: |-
    Sets the value of the specified comment's property.

    You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-delete
  description: Removes the property from the comment identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Bulk set issue property
  x-api-slug: api2issuepropertiespropertykey-put
  description: |-
    Allows to set a property for all issues identified by a given filter. Only entities the user has permissions to edit will be updated.

    Currently the following filters are available:

    *   **entityIds** \- A list of issues to update. Only issues with ids from this list will be considered for updating. This is an optional filter, if not provided, then any editable issue that matches all other filters will be updated.
    *   **currentValue** \- If provided, then only issues with the property currently set to that value will be updated.
    *   **hasProperty** \- If true, then only existing properties will be updated. If false, then only issues that do not have any value associated with this property will be updated. If omitted, the property will be set on all issues, regardless of whether it previously existed or not.

    If more than one filter is given, then they are all joined with the logical "and", that is: only issues that satisfy all filters are updated. If no filters are provided at all, then the property will be updated on _all_ issues editable by the caller (i.e. issues in projects with the EDIT_ISSUES permission).

    If an invalid combination of filters is provided, an error will be returned by the API. For example, specifying the current value and "hasProperty" to "false" would never match any issues (as it would mean: update this property if the current value is something, oh, but only if there is no value at all) and is therefore not allowed.

    This method is [asynchronous](#async), meaning that it will not return the results immediately, instead creating a task to perform the requested update operation (unless preliminary validation, e.g. of the provided filter, fails).

    The operation is transactional: either all eligible issues are updated, or none (if there are any errors).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Bulk delete issue property
  x-api-slug: api2issuepropertiespropertykey-delete
  description: Allows to delete a property from all issues identified by a given filter.
    Only entities the user has permissions to edit will be updated. See the [issue
    property bulk set endpoint documentation](#api-api-2-issue-properties-propertyKey-put)
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get issue property keys
  x-api-slug: api2issueissueidorkeyproperties-get
  description: Returns the keys of all properties for the issue identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Get issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-get
  description: Returns the value of the property with a given key from the issue identified
    by the key or by the id. The user who retrieves the property is required to have
    permissions to read the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the specified issue's property.

    You can use this resource to store a custom data against the issue identified by the key or by the id. The user who stores the data is required to have permissions to edit the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-delete
  description: Removes the property from the issue identified by the key or by the
    id. Ths user removing the property is required to have permissions to edit the
    issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get worklog property keys
  x-api-slug: api2issueissueidorkeyworklogworklogidproperties-get
  description: Returns the keys of all properties for the worklog identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-openapi.md
- name: Jira Cloud REST API - Get worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the worklog
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-put
  description: |-
    Sets the value of the specified worklog's property.

    You can use this resource to store a custom data against the worklog identified by the key or by the id. The user who stores the data is required to have permissions to administer the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
  description: Removes the property from the worklog identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get issue type property keys
  x-api-slug: api2issuetypeissuetypeidproperties-get
  description: |-
    Returns all the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys of the issue type. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   _Administer Jira_ [global permission](href=) to get the property keys of any issue type.
    *   _Browse projects_ project permission to get the property keys of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-openapi.md
- name: Jira Cloud REST API - Get issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-get
  description: |-
    Returns the key and value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:

    *   _Administer Jira_ [global permission](href=) to get the details of any issue type.
    *   _Browse projects_ project permission to get the details of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-put
  description: Creates or updates the value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    Use this resource to store and update data against an issue type. The value of
    the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty
    JSON blob. The maximum length of the property value is 32768 bytes. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** _Administer Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-delete
  description: Deletes the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer
    Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get project property keys
  x-api-slug: api2projectprojectidorkeyproperties-get
  description: |-
    Returns all [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys for the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Get project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-get
  description: |-
    Returns the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). You can use project properties to store custom data against the project.

    The value of the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob. The maximum length is 32768 bytes.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-delete
  description: |-
    Removes the [property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) from the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Get application property
  x-api-slug: api2applicationproperties-get
  description: Returns an application property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-openapi.md
- name: Jira Cloud REST API - Set application property
  x-api-slug: api2applicationpropertiesid-put
  description: Modify an application property via PUT. The "value" field present in
    the PUT will override the existing value.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-openapi.md
- name: Jira Cloud REST API - Get comment property keys
  x-api-slug: api2commentcommentidproperties-get
  description: Returns the keys of all properties for the comment identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-openapi.md
- name: Jira Cloud REST API - Get comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the comment
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-put
  description: |-
    Sets the value of the specified comment's property.

    You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-delete
  description: Removes the property from the comment identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Bulk set issue property
  x-api-slug: api2issuepropertiespropertykey-put
  description: |-
    Allows to set a property for all issues identified by a given filter. Only entities the user has permissions to edit will be updated.

    Currently the following filters are available:

    *   **entityIds** \- A list of issues to update. Only issues with ids from this list will be considered for updating. This is an optional filter, if not provided, then any editable issue that matches all other filters will be updated.
    *   **currentValue** \- If provided, then only issues with the property currently set to that value will be updated.
    *   **hasProperty** \- If true, then only existing properties will be updated. If false, then only issues that do not have any value associated with this property will be updated. If omitted, the property will be set on all issues, regardless of whether it previously existed or not.

    If more than one filter is given, then they are all joined with the logical "and", that is: only issues that satisfy all filters are updated. If no filters are provided at all, then the property will be updated on _all_ issues editable by the caller (i.e. issues in projects with the EDIT_ISSUES permission).

    If an invalid combination of filters is provided, an error will be returned by the API. For example, specifying the current value and "hasProperty" to "false" would never match any issues (as it would mean: update this property if the current value is something, oh, but only if there is no value at all) and is therefore not allowed.

    This method is [asynchronous](#async), meaning that it will not return the results immediately, instead creating a task to perform the requested update operation (unless preliminary validation, e.g. of the provided filter, fails).

    The operation is transactional: either all eligible issues are updated, or none (if there are any errors).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Bulk delete issue property
  x-api-slug: api2issuepropertiespropertykey-delete
  description: Allows to delete a property from all issues identified by a given filter.
    Only entities the user has permissions to edit will be updated. See the [issue
    property bulk set endpoint documentation](#api-api-2-issue-properties-propertyKey-put)
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get issue property keys
  x-api-slug: api2issueissueidorkeyproperties-get
  description: Returns the keys of all properties for the issue identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Get issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-get
  description: Returns the value of the property with a given key from the issue identified
    by the key or by the id. The user who retrieves the property is required to have
    permissions to read the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the specified issue's property.

    You can use this resource to store a custom data against the issue identified by the key or by the id. The user who stores the data is required to have permissions to edit the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-delete
  description: Removes the property from the issue identified by the key or by the
    id. Ths user removing the property is required to have permissions to edit the
    issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get worklog property keys
  x-api-slug: api2issueissueidorkeyworklogworklogidproperties-get
  description: Returns the keys of all properties for the worklog identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-openapi.md
- name: Jira Cloud REST API - Get worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the worklog
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-put
  description: |-
    Sets the value of the specified worklog's property.

    You can use this resource to store a custom data against the worklog identified by the key or by the id. The user who stores the data is required to have permissions to administer the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
  description: Removes the property from the worklog identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get issue type property keys
  x-api-slug: api2issuetypeissuetypeidproperties-get
  description: |-
    Returns all the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys of the issue type. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   _Administer Jira_ [global permission](href=) to get the property keys of any issue type.
    *   _Browse projects_ project permission to get the property keys of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-openapi.md
- name: Jira Cloud REST API - Get issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-get
  description: |-
    Returns the key and value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:

    *   _Administer Jira_ [global permission](href=) to get the details of any issue type.
    *   _Browse projects_ project permission to get the details of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-put
  description: Creates or updates the value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    Use this resource to store and update data against an issue type. The value of
    the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty
    JSON blob. The maximum length of the property value is 32768 bytes. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** _Administer Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-delete
  description: Deletes the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer
    Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get project property keys
  x-api-slug: api2projectprojectidorkeyproperties-get
  description: |-
    Returns all [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys for the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Get project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-get
  description: |-
    Returns the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). You can use project properties to store custom data against the project.

    The value of the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob. The maximum length is 32768 bytes.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-delete
  description: |-
    Removes the [property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) from the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-delete
  description: |-
    Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-delete-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Update workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-put
  description: |-
    Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-put-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Create workflow transition property
  x-api-slug: api2workflowtransitionstransitionidproperties-post
  description: |-
    Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2workflowtransitionstransitionidproperties-post-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete user property
  x-api-slug: api2userpropertiespropertykey-delete
  description: |-
    Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To delete a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set user property
  x-api-slug: api2userpropertiespropertykey-put
  description: |-
    Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To set a property on the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get user property
  x-api-slug: api2userpropertiespropertykey-get
  description: |-
    Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To get a property from the calling user's record: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Get user property keys
  x-api-slug: api2userproperties-get
  description: |-
    Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
    *   To access the calling user's property keys: None

    Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2userproperties-get-openapi.md
- name: Jira Cloud REST API - Delete project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-delete
  description: |-
    Removes the [property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) from the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). You can use project properties to store custom data against the project.

    The value of the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob. The maximum length is 32768 bytes.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-get
  description: |-
    Returns the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get project property keys
  x-api-slug: api2projectprojectidorkeyproperties-get
  description: |-
    Returns all [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys for the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Get project property keys
  x-api-slug: api2projectprojectidorkeyproperties-get
  description: |-
    Returns all [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys for the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2projectprojectidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Delete issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-delete
  description: Deletes the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer
    Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-delete
  description: Deletes the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer
    Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-put
  description: Creates or updates the value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    Use this resource to store and update data against an issue type. The value of
    the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty
    JSON blob. The maximum length of the property value is 32768 bytes. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** _Administer Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-put
  description: Creates or updates the value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
    Use this resource to store and update data against an issue type. The value of
    the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty
    JSON blob. The maximum length of the property value is 32768 bytes. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** _Administer Jira_ [global permission](href=).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-get
  description: |-
    Returns the key and value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:

    *   _Administer Jira_ [global permission](href=) to get the details of any issue type.
    *   _Browse projects_ project permission to get the details of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get issue type property
  x-api-slug: api2issuetypeissuetypeidpropertiespropertykey-get
  description: |-
    Returns the key and value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:

    *   _Administer Jira_ [global permission](href=) to get the details of any issue type.
    *   _Browse projects_ project permission to get the details of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get issue type property keys
  x-api-slug: api2issuetypeissuetypeidproperties-get
  description: |-
    Returns all the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys of the issue type. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   _Administer Jira_ [global permission](href=) to get the property keys of any issue type.
    *   _Browse projects_ project permission to get the property keys of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-openapi.md
- name: Jira Cloud REST API - Get issue type property keys
  x-api-slug: api2issuetypeissuetypeidproperties-get
  description: |-
    Returns all the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys of the issue type. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   _Administer Jira_ [global permission](href=) to get the property keys of any issue type.
    *   _Browse projects_ project permission to get the property keys of any issue types associated with the projects the user has permission to browse.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuetypeissuetypeidproperties-get-openapi.md
- name: Jira Cloud REST API - Delete worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
  description: Removes the property from the worklog identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
  description: Removes the property from the worklog identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-put
  description: |-
    Sets the value of the specified worklog's property.

    You can use this resource to store a custom data against the worklog identified by the key or by the id. The user who stores the data is required to have permissions to administer the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-put
  description: |-
    Sets the value of the specified worklog's property.

    You can use this resource to store a custom data against the worklog identified by the key or by the id. The user who stores the data is required to have permissions to administer the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the worklog
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the worklog
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get worklog property keys
  x-api-slug: api2issueissueidorkeyworklogworklogidproperties-get
  description: Returns the keys of all properties for the worklog identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-openapi.md
- name: Jira Cloud REST API - Get worklog property keys
  x-api-slug: api2issueissueidorkeyworklogworklogidproperties-get
  description: Returns the keys of all properties for the worklog identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidproperties-get-openapi.md
- name: Jira Cloud REST API - Delete issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-delete
  description: Removes the property from the issue identified by the key or by the
    id. Ths user removing the property is required to have permissions to edit the
    issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-delete
  description: Removes the property from the issue identified by the key or by the
    id. Ths user removing the property is required to have permissions to edit the
    issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the specified issue's property.

    You can use this resource to store a custom data against the issue identified by the key or by the id. The user who stores the data is required to have permissions to edit the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-put
  description: |-
    Sets the value of the specified issue's property.

    You can use this resource to store a custom data against the issue identified by the key or by the id. The user who stores the data is required to have permissions to edit the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-get
  description: Returns the value of the property with a given key from the issue identified
    by the key or by the id. The user who retrieves the property is required to have
    permissions to read the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-get
  description: Returns the value of the property with a given key from the issue identified
    by the key or by the id. The user who retrieves the property is required to have
    permissions to read the issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get issue property keys
  x-api-slug: api2issueissueidorkeyproperties-get
  description: Returns the keys of all properties for the issue identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Get issue property keys
  x-api-slug: api2issueissueidorkeyproperties-get
  description: Returns the keys of all properties for the issue identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issueissueidorkeyproperties-get-openapi.md
- name: Jira Cloud REST API - Bulk delete issue property
  x-api-slug: api2issuepropertiespropertykey-delete
  description: Allows to delete a property from all issues identified by a given filter.
    Only entities the user has permissions to edit will be updated. See the [issue
    property bulk set endpoint documentation](#api-api-2-issue-properties-propertyKey-put)
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Bulk delete issue property
  x-api-slug: api2issuepropertiespropertykey-delete
  description: Allows to delete a property from all issues identified by a given filter.
    Only entities the user has permissions to edit will be updated. See the [issue
    property bulk set endpoint documentation](#api-api-2-issue-properties-propertyKey-put)
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Bulk set issue property
  x-api-slug: api2issuepropertiespropertykey-put
  description: |-
    Allows to set a property for all issues identified by a given filter. Only entities the user has permissions to edit will be updated.

    Currently the following filters are available:

    *   **entityIds** \- A list of issues to update. Only issues with ids from this list will be considered for updating. This is an optional filter, if not provided, then any editable issue that matches all other filters will be updated.
    *   **currentValue** \- If provided, then only issues with the property currently set to that value will be updated.
    *   **hasProperty** \- If true, then only existing properties will be updated. If false, then only issues that do not have any value associated with this property will be updated. If omitted, the property will be set on all issues, regardless of whether it previously existed or not.

    If more than one filter is given, then they are all joined with the logical "and", that is: only issues that satisfy all filters are updated. If no filters are provided at all, then the property will be updated on _all_ issues editable by the caller (i.e. issues in projects with the EDIT_ISSUES permission).

    If an invalid combination of filters is provided, an error will be returned by the API. For example, specifying the current value and "hasProperty" to "false" would never match any issues (as it would mean: update this property if the current value is something, oh, but only if there is no value at all) and is therefore not allowed.

    This method is [asynchronous](#async), meaning that it will not return the results immediately, instead creating a task to perform the requested update operation (unless preliminary validation, e.g. of the provided filter, fails).

    The operation is transactional: either all eligible issues are updated, or none (if there are any errors).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Bulk set issue property
  x-api-slug: api2issuepropertiespropertykey-put
  description: |-
    Allows to set a property for all issues identified by a given filter. Only entities the user has permissions to edit will be updated.

    Currently the following filters are available:

    *   **entityIds** \- A list of issues to update. Only issues with ids from this list will be considered for updating. This is an optional filter, if not provided, then any editable issue that matches all other filters will be updated.
    *   **currentValue** \- If provided, then only issues with the property currently set to that value will be updated.
    *   **hasProperty** \- If true, then only existing properties will be updated. If false, then only issues that do not have any value associated with this property will be updated. If omitted, the property will be set on all issues, regardless of whether it previously existed or not.

    If more than one filter is given, then they are all joined with the logical "and", that is: only issues that satisfy all filters are updated. If no filters are provided at all, then the property will be updated on _all_ issues editable by the caller (i.e. issues in projects with the EDIT_ISSUES permission).

    If an invalid combination of filters is provided, an error will be returned by the API. For example, specifying the current value and "hasProperty" to "false" would never match any issues (as it would mean: update this property if the current value is something, oh, but only if there is no value at all) and is therefore not allowed.

    This method is [asynchronous](#async), meaning that it will not return the results immediately, instead creating a task to perform the requested update operation (unless preliminary validation, e.g. of the provided filter, fails).

    The operation is transactional: either all eligible issues are updated, or none (if there are any errors).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2issuepropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Delete comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-delete
  description: Removes the property from the comment identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-delete
  description: Removes the property from the comment identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-put
  description: |-
    Sets the value of the specified comment's property.

    You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-put
  description: |-
    Sets the value of the specified comment's property.

    You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the comment
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-get
  description: Returns the value of the property with a given key from the comment
    identified by the key or by the id. The user who retrieves the property is required
    to have permissions to read the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get comment property keys
  x-api-slug: api2commentcommentidproperties-get
  description: Returns the keys of all properties for the comment identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-openapi.md
- name: Jira Cloud REST API - Get comment property keys
  x-api-slug: api2commentcommentidproperties-get
  description: Returns the keys of all properties for the comment identified by the
    key or by the id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2commentcommentidproperties-get-openapi.md
- name: Jira Cloud REST API - Set application property
  x-api-slug: api2applicationpropertiesid-put
  description: Modify an application property via PUT. The "value" field present in
    the PUT will override the existing value.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-openapi.md
- name: Jira Cloud REST API - Set application property
  x-api-slug: api2applicationpropertiesid-put
  description: Modify an application property via PUT. The "value" field present in
    the PUT will override the existing value.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationpropertiesid-put-openapi.md
- name: Jira Cloud REST API - Get application property
  x-api-slug: api2applicationproperties-get
  description: Returns an application property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-openapi.md
- name: Jira Cloud REST API - Get application property
  x-api-slug: api2applicationproperties-get
  description: Returns an application property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/atlassian/api2applicationproperties-get-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---