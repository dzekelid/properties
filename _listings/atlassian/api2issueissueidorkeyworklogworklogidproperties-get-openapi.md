---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get worklog property keys
  description: Returns the keys of all properties for the worklog identified by the
    key or by the id.
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
  /api/2/workflow/transitions/{transitionId}/properties:
    get:
      summary: Get workflow transition properties
      description: |-
        Returns the properties on a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.getWorkflowTransitionProperties_get
      x-api-path-slug: api2workflowtransitionstransitionidproperties-get
      parameters:
      - in: query
        name: includeReservedKeys
        description: Some properties with keys that have the _jira
      - in: query
        name: key
        description: The key of the property being returned, also known as the name
          of the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Properties
    post:
      summary: Create workflow transition property
      description: |-
        Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.createWorkflowTransitionProperty_post
      x-api-path-slug: api2workflowtransitionstransitionidproperties-post
      parameters:
      - in: query
        name: key
        description: The key of the property being added, also known as the name of
          the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Property
    put:
      summary: Update workflow transition property
      description: |-
        Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.updateWorkflowTransitionProperty_put
      x-api-path-slug: api2workflowtransitionstransitionidproperties-put
      parameters:
      - in: query
        name: key
        description: The key of the property being updated, also known as the name
          of the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Property
    delete:
      summary: Delete workflow transition property
      description: |-
        Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.deleteWorkflowTransitionProperty_delete
      x-api-path-slug: api2workflowtransitionstransitionidproperties-delete
      parameters:
      - in: query
        name: key
        description: The name of the transition property to delete, also known as
          the name of the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Property
  /api/2/application-properties:
    get:
      summary: Get application property
      description: Returns an application property.
      operationId: com.atlassian.jira.rest.v2.admin.ApplicationPropertiesResource.getApplicationProperty_get
      x-api-path-slug: api2applicationproperties-get
      parameters:
      - in: query
        name: key
        description: a String containing the property key
      - in: query
        name: keyFilter
        description: when fetching a list allows the list to be filtered by the propertys
          start of key e
      - in: query
        name: permissionLevel
        description: when fetching a list specifies the permission level of all items
          in the list see {@link com
      responses:
        200:
          description: OK
      tags:
      - Application
      - Property
  /api/2/application-properties/{id}:
    put:
      summary: Set application property
      description: Modify an application property via PUT. The "value" field present
        in the PUT will override the existing value.
      operationId: com.atlassian.jira.rest.v2.admin.ApplicationPropertiesResource.setApplicationProperty_put
      x-api-path-slug: api2applicationpropertiesid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Set
      - Application
      - Property
  /api/2/comment/{commentId}/properties:
    get:
      summary: Get comment property keys
      description: Returns the keys of all properties for the comment identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.getCommentPropertyKeys_get
      x-api-path-slug: api2commentcommentidproperties-get
      parameters:
      - in: path
        name: commentId
        description: the comment from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
      - Keys
  /api/2/comment/{commentId}/properties/{propertyKey}:
    get:
      summary: Get comment property
      description: Returns the value of the property with a given key from the comment
        identified by the key or by the id. The user who retrieves the property is
        required to have permissions to read the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.getCommentProperty_get
      x-api-path-slug: api2commentcommentidpropertiespropertykey-get
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be returned
      - in: path
        name: propertyKey
        description: the key of the property to return
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
    put:
      summary: Set comment property
      description: |-
        Sets the value of the specified comment's property.

        You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.setCommentProperty_put
      x-api-path-slug: api2commentcommentidpropertiespropertykey-put
      parameters:
      - in: path
        name: commentId
        description: the comment on which the property will be set
      - in: path
        name: propertyKey
        description: the key of the comments property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Comment
      - Property
    delete:
      summary: Delete comment property
      description: Removes the property from the comment identified by the key or
        by the id. Ths user removing the property is required to have permissions
        to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.deleteCommentProperty_delete
      x-api-path-slug: api2commentcommentidpropertiespropertykey-delete
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be removed
      - in: path
        name: propertyKey
        description: the key of the property to remove
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
  /api/2/dashboard/{dashboardId}/items/{itemId}/properties:
    get:
      summary: Get dashboard item property keys
      description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira. However, to get the property keys the
        user must be the owner of the dashboard or be shared the dashboard. Note,
        users with the _Administer Jira_ [global permission](href=) are considered
        owners of the System dashboard. The System dashboard is considered to be shared
        with all other users."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.getDashboardItemPropertyKeys_get
      x-api-path-slug: api2dashboarddashboardiditemsitemidproperties-get
      parameters:
      - in: path
        name: dashboardId
        description: The ID of the dashboard
      - in: path
        name: itemId
        description: The ID of the dashboard item
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Item
      - Property
      - Keys
  /api/2/dashboard/{dashboardId}/items/{itemId}/properties/{propertyKey}:
    get:
      summary: Get dashboard item property
      description: "Returns the key and value of a dashboard item property.  \n  \nA
        dashboard item enables an app to add user-specific information to a user dashboard.
        Dashboard items are exposed to users as gadgets that users can add to their
        dashboards. For more information on how users do this, see [Adding and customizing
        gadgets](https://confluence.atlassian.com/x/7AeiLQ).  \n  \nWhen an app creates
        a dashboard item it registers a callback to receive the dashboard item ID.
        The callback fires whenever the item is rendered or, where the item is configurable,
        the user edits the item. The app then uses this resource to store the item's
        content or configuration details. For more information on working with dashboard
        items, see [Building a dashboard item for a JIRA Connect add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
        and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
        documentation.  \n  \nThere is no resource to set or get dashboard items.
        \ \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        Permission to access Jira. However, to get a dashboard item property the user
        must be the owner of the dashboard or be shared the dashboard. Note, users
        with the _Administer Jira_ [global permission](href=) are considered owners
        of the System dashboard. The System dashboard is considered to be shared with
        all other users."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.getDashboardItemProperty_get
      x-api-path-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
      parameters:
      - in: path
        name: dashboardId
        description: The ID of the dashboard
      - in: path
        name: itemId
        description: The ID of the dashboard item
      - in: path
        name: propertyKey
        description: The key of the dashboard item property
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Item
      - Property
    put:
      summary: Set dashboard item property
      description: "Sets the value of a dashboard item property. Use this resource
        in apps to store custom data against a dashboard item.  \n  \nA dashboard
        item enables an app to add user-specific information to a user dashboard.
        Dashboard items are exposed to users as gadgets that users can add to their
        dashboards. For more information on how users do this, see [Adding and customizing
        gadgets](https://confluence.atlassian.com/x/7AeiLQ).  \n  \nWhen an app creates
        a dashboard item it registers a callback to receive the dashboard item ID.
        The callback fires whenever the item is rendered or, where the item is configurable,
        the user edits the item. The app then uses this resource to store the item's
        content or configuration details. For more information on working with dashboard
        items, see [Building a dashboard item for a JIRA Connect add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
        and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
        documentation.  \n  \nThere is no resource to set or get dashboard items.
        \ \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        Permission to access Jira. However, to set a dashboard item property the user
        must be the owner of the dashboard. Note, users with the _Administer Jira_
        [global permission](href=) are considered owners of the System dashboard.
        \ \n  \nThe value of the request body must be a [valid](http://tools.ietf.org/html/rfc4627),
        non-empty JSON blob. The maximum length is 32768 bytes."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.setDashboardItemProperty_put
      x-api-path-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
      parameters:
      - in: path
        name: dashboardId
        description: The ID of the dashboard
      - in: path
        name: itemId
        description: The ID of the dashboard item
      - in: path
        name: propertyKey
        description: The key of the dashboard item property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Dashboard
      - Item
      - Property
    delete:
      summary: Delete dashboard item property
      description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira. However, to delete a dashboard item
        property the user must be the owner of the dashboard. Note, users with the
        _Administer Jira_ [global permission](href=) are considered owners of the
        System dashboard."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.deleteDashboardItemProperty_delet
      x-api-path-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
      parameters:
      - in: path
        name: dashboardId
        description: The ID of the dashboard
      - in: path
        name: itemId
        description: The ID of the dashboard item
      - in: path
        name: propertyKey
        description: The key of the dashboard item property
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Item
      - Property
  /api/2/issue/properties/{propertyKey}:
    put:
      summary: Bulk set issue property
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
      operationId: com.atlassian.jira.rest.v2.property.IssuePropertyBulkUpdateResource.bulkSetIssueProperty_put
      x-api-path-slug: api2issuepropertiespropertykey-put
      parameters:
      - in: path
        name: propertyKey
        description: The key of the property to update
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Set
      - Issue
      - Property
    delete:
      summary: Bulk delete issue property
      description: Allows to delete a property from all issues identified by a given
        filter. Only entities the user has permissions to edit will be updated. See
        the [issue property bulk set endpoint documentation](#api-api-2-issue-properties-propertyKey-put)
        for more details.
      operationId: com.atlassian.jira.rest.v2.property.IssuePropertyBulkUpdateResource.bulkDeleteIssueProperty_delete
      x-api-path-slug: api2issuepropertiespropertykey-delete
      parameters:
      - in: path
        name: propertyKey
        description: The key of the property to delete
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Delete
      - Issue
      - Property
  /api/2/issue/{issueIdOrKey}/properties:
    get:
      summary: Get issue property keys
      description: Returns the keys of all properties for the issue identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.getIssuePropertyKeys_get
      x-api-path-slug: api2issueissueidorkeyproperties-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Property
      - Keys
  /api/2/issue/{issueIdOrKey}/properties/{propertyKey}:
    get:
      summary: Get issue property
      description: Returns the value of the property with a given key from the issue
        identified by the key or by the id. The user who retrieves the property is
        required to have permissions to read the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.getIssueProperty_get
      x-api-path-slug: api2issueissueidorkeypropertiespropertykey-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue from which the property will be returned
      - in: path
        name: propertyKey
        description: the key of the property to return
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Property
    put:
      summary: Set issue property
      description: |-
        Sets the value of the specified issue's property.

        You can use this resource to store a custom data against the issue identified by the key or by the id. The user who stores the data is required to have permissions to edit the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.setIssueProperty_put
      x-api-path-slug: api2issueissueidorkeypropertiespropertykey-put
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue on which the property will be set
      - in: path
        name: propertyKey
        description: the key of the issues property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Issue
      - Property
    delete:
      summary: Delete issue property
      description: Removes the property from the issue identified by the key or by
        the id. Ths user removing the property is required to have permissions to
        edit the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.deleteIssueProperty_delete
      x-api-path-slug: api2issueissueidorkeypropertiespropertykey-delete
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue from which the property will be removed
      - in: path
        name: propertyKey
        description: the key of the property to remove
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Property
  /api/2/issue/{issueIdOrKey}/worklog/{worklogId}/properties:
    get:
      summary: Get worklog property keys
      description: Returns the keys of all properties for the worklog identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.WorklogPropertyResource.getWorklogPropertyKeys_get
      x-api-path-slug: api2issueissueidorkeyworklogworklogidproperties-get
      parameters:
      - in: path
        name: issueIdOrKey
      - in: path
        name: worklogId
        description: the worklog from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Worklog
      - Property
      - Keys
  /api/2/issue/{issueIdOrKey}/worklog/{worklogId}/properties/{propertyKey}:
    get:
      summary: Get worklog property
      description: Returns the value of the property with a given key from the worklog
        identified by the key or by the id. The user who retrieves the property is
        required to have permissions to read the worklog.
      operationId: com.atlassian.jira.rest.v2.issue.WorklogPropertyResource.getWorklogProperty_get
      x-api-path-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-get
      parameters:
      - in: path
        name: issueIdOrKey
      - in: path
        name: propertyKey
        description: the key of the property to return
      - in: path
        name: worklogId
        description: the worklog from which the property will be returned
      responses:
        200:
          description: OK
      tags:
      - Worklog
      - Property
    put:
      summary: Set worklog property
      description: |-
        Sets the value of the specified worklog's property.

        You can use this resource to store a custom data against the worklog identified by the key or by the id. The user who stores the data is required to have permissions to administer the worklog.
      operationId: com.atlassian.jira.rest.v2.issue.WorklogPropertyResource.setWorklogProperty_put
      x-api-path-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-put
      parameters:
      - in: path
        name: issueIdOrKey
      - in: path
        name: propertyKey
        description: the key of the worklogs property
      - in: path
        name: worklogId
        description: the worklog on which the property will be set
      responses:
        200:
          description: OK
      tags:
      - Set
      - Worklog
      - Property
    delete:
      summary: Delete worklog property
      description: Removes the property from the worklog identified by the key or
        by the id. Ths user removing the property is required to have permissions
        to administer the worklog.
      operationId: com.atlassian.jira.rest.v2.issue.WorklogPropertyResource.deleteWorklogProperty_delete
      x-api-path-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
      parameters:
      - in: path
        name: issueIdOrKey
      - in: path
        name: propertyKey
        description: the key of the property to remove
      - in: path
        name: worklogId
        description: the worklog from which the property will be removed
      responses:
        200:
          description: OK
      tags:
      - Worklog
      - Property
  /api/2/issuetype/{issueTypeId}/properties:
    get:
      summary: Get issue type property keys
      description: |-
        Returns all the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys of the issue type. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   _Administer Jira_ [global permission](href=) to get the property keys of any issue type.
        *   _Browse projects_ project permission to get the property keys of any issue types associated with the projects the user has permission to browse.
      operationId: com.atlassian.jira.rest.v2.issue.IssueTypePropertyResource.getIssueTypePropertyKeys_get
      x-api-path-slug: api2issuetypeissuetypeidproperties-get
      parameters:
      - in: path
        name: issueTypeId
        description: The ID of the issue type
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Type
      - Property
      - Keys
  /api/2/issuetype/{issueTypeId}/properties/{propertyKey}:
    get:
      summary: Get issue type property
      description: |-
        Returns the key and value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). [Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:

        *   _Administer Jira_ [global permission](href=) to get the details of any issue type.
        *   _Browse projects_ project permission to get the details of any issue types associated with the projects the user has permission to browse.
      operationId: com.atlassian.jira.rest.v2.issue.IssueTypePropertyResource.getIssueTypeProperty_get
      x-api-path-slug: api2issuetypeissuetypeidpropertiespropertykey-get
      parameters:
      - in: path
        name: issueTypeId
        description: The ID of the issue type
      - in: path
        name: propertyKey
        description: The key of the property
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Type
      - Property
    put:
      summary: Set issue type property
      description: Creates or updates the value of the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
        Use this resource to store and update data against an issue type. The value
        of the request body must be a [valid](http://tools.ietf.org/html/rfc4627),
        non-empty JSON blob. The maximum length of the property value is 32768 bytes.
        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer
        Jira_ [global permission](href=).
      operationId: com.atlassian.jira.rest.v2.issue.IssueTypePropertyResource.setIssueTypeProperty_put
      x-api-path-slug: api2issuetypeissuetypeidpropertiespropertykey-put
      parameters:
      - in: path
        name: issueTypeId
        description: The ID of the issue type
      - in: path
        name: propertyKey
        description: The key of the issue type property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Issue
      - Type
      - Property
    delete:
      summary: Delete issue type property
      description: Deletes the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).
        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer
        Jira_ [global permission](href=).
      operationId: com.atlassian.jira.rest.v2.issue.IssueTypePropertyResource.deleteIssueTypeProperty_delete
      x-api-path-slug: api2issuetypeissuetypeidpropertiespropertykey-delete
      parameters:
      - in: path
        name: issueTypeId
        description: The ID of the issue type
      - in: path
        name: propertyKey
        description: The key of the property
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Type
      - Property
  /api/2/project/{projectIdOrKey}/properties:
    get:
      summary: Get project property keys
      description: |-
        Returns all [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys for the project.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectPropertyResource.getProjectPropertyKeys_get
      x-api-path-slug: api2projectprojectidorkeyproperties-get
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Project
      - Property
      - Keys
  /api/2/project/{projectIdOrKey}/properties/{propertyKey}:
    get:
      summary: Get project property
      description: |-
        Returns the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectPropertyResource.getProjectProperty_get
      x-api-path-slug: api2projectprojectidorkeypropertiespropertykey-get
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: path
        name: propertyKey
        description: The project property key
      responses:
        200:
          description: OK
      tags:
      - Project
      - Property
    put:
      summary: Set project property
      description: |-
        Sets the value of the [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties). You can use project properties to store custom data against the project.

        The value of the request body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob. The maximum length is 32768 bytes.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectPropertyResource.setProjectProperty_put
      x-api-path-slug: api2projectprojectidorkeypropertiespropertykey-put
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: path
        name: propertyKey
        description: The key of the project property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Project
      - Property
    delete:
      summary: Delete project property
      description: |-
        Removes the [property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) from the project.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectPropertyResource.deleteProjectProperty_delete
      x-api-path-slug: api2projectprojectidorkeypropertiespropertykey-delete
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: path
        name: propertyKey
        description: The project property key
      responses:
        200:
          description: OK
      tags:
      - Project
      - Property
  /api/2/user/properties:
    get:
      summary: Get user property keys
      description: |-
        Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To access the calling user's property keys: None

        Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
      operationId: com.atlassian.jira.rest.v2.userproperty.UserPropertyResource.getUserPropertyKeys_get
      x-api-path-slug: api2userproperties-get
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user
      - in: header
        name: force-account-id
      - in: query
        name: userKey
        description: The key of the user
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - Property
      - Keys
  /api/2/user/properties/{propertyKey}:
    get:
      summary: Get user property
      description: |-
        Returns the value of a user's property. If no property key is provided [Get user property keys](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-user-properties-get) is called. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To get a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To get a property from the calling user's record: None

        Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
      operationId: com.atlassian.jira.rest.v2.userproperty.UserPropertyResource.getUserProperty_get
      x-api-path-slug: api2userpropertiespropertykey-get
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user
      - in: header
        name: force-account-id
      - in: path
        name: propertyKey
        description: The key of the users property
      - in: query
        name: userKey
        description: The key of the user
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - Property
    put:
      summary: Set user property
      description: |-
        Sets the value of a user's property. Use this resource to store custom data against a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To set a property on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To set a property on the calling user's record: None

        Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
      operationId: com.atlassian.jira.rest.v2.userproperty.UserPropertyResource.setUserProperty_put
      x-api-path-slug: api2userpropertiespropertykey-put
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user
      - in: header
        name: force-account-id
      - in: path
        name: propertyKey
        description: The key of the users property
      - in: query
        name: userKey
        description: The key of the user
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - Set
      - User
      - Property
    delete:
      summary: Delete user property
      description: |-
        Deletes a property from a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To delete a property from any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To delete a property from the calling user's record: None

        Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
      operationId: com.atlassian.jira.rest.v2.userproperty.UserPropertyResource.deleteUserProperty_delete
      x-api-path-slug: api2userpropertiespropertykey-delete
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user
      - in: header
        name: force-account-id
      - in: path
        name: propertyKey
        description: The key of the users property
      - in: query
        name: userKey
        description: The key of the user
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - User
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