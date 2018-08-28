---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List property selections
  description: Lists property selections
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/properties:
    get:
      summary: List properties
      description: Lists all properties.
      operationId: getRestItemsProperties
      x-api-path-slug: restitemsproperties-get
      parameters:
      - in: query
        name: groupId
        description: Filter restricts the list of results to items linked to a specified
          property group
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified property information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
    post:
      summary: Create a property
      description: Creates a property.
      operationId: postRestItemsProperties
      x-api-path-slug: restitemsproperties-post
      parameters:
      - in: body
        name: /rest/items/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/items/variations/variation_properties:
    post:
      summary: Bulk update properties
      description: Creates up to 50 properties of variations.
      operationId: postRestItemsVariationsVariationProperties
      x-api-path-slug: restitemsvariationsvariation-properties-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Properties
    put:
      summary: Bulk update properties
      description: Updates up to 50 properties of variations.
      operationId: putRestItemsVariationsVariationProperties
      x-api-path-slug: restitemsvariationsvariation-properties-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Properties
  /rest/orders/{orderId}/properties/{typeId?}:
    get:
      summary: List properties of an order
      description: Lists properties of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: typeId
        description: The property type ID
      - in: path
        name: typeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - Of
      - Order
  /rest/payments/properties:
    get:
      summary: List properties
      description: List properties.
      operationId: getRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
    post:
      summary: Create a payment property
      description: Create a payment property.
      operationId: postRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-post
      parameters:
      - in: body
        name: /rest/payments/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Property
    put:
      summary: Update a payment property
      description: Update a payment property.
      operationId: putRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-put
      parameters:
      - in: body
        name: /rest/payments/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Property
  /rest/payments/properties/date:
    get:
      summary: List properties by creation date
      description: Lists all properties by creation date. The start and the end of
        the date range must be specified.
      operationId: getRestPaymentsPropertiesDate
      x-api-path-slug: restpaymentspropertiesdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the date of creation of the
          property
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the date of creation of
          the property
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - By
      - Creation
      - Date
  /rest/properties:
    get:
      summary: List properties
      description: Lists properties.
      operationId: getRestProperties
      x-api-path-slug: restproperties-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
    post:
      summary: Create a property
      description: Creates a property
      operationId: postRestProperties
      x-api-path-slug: restproperties-post
      parameters:
      - in: body
        name: /rest/properties
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: cast
        description: The cast of the property
      - in: query
        name: position
        description: The position of the property
      - in: query
        name: typeIdentifier
        description: The identifier of the property type
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/payments/{paymentId}/properties:
    get:
      summary: List properties for a payment
      description: Lists all properties for a payment. The ID of the payment must
        be specified.
      operationId: getRestPaymentsPaymentProperties
      x-api-path-slug: restpaymentspaymentidproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - List
      - Propertiesa
      - Payment
  /rest/items/properties/{id}:
    delete:
      summary: Delete a property
      description: Deletes a property. The ID of the property must be specified.
      operationId: deleteRestItemsProperties
      x-api-path-slug: restitemspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
    get:
      summary: Get a property
      description: Gets a property. The ID of the property must be specified.
      operationId: getRestItemsProperties
      x-api-path-slug: restitemspropertiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
    put:
      summary: Update a property
      description: Updates a property. The ID of the property must be specified.
      operationId: putRestItemsProperties
      x-api-path-slug: restitemspropertiesid-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/items/properties/{id}/market_references:
    get:
      summary: List property market references
      description: Lists the property market references of a property. The ID of the
        property must be specified.
      operationId: getRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Market
      - References
    post:
      summary: Create a property market reference
      description: Creates a property market reference.
      operationId: postRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-post
      parameters:
      - in: body
        name: /rest/items/properties/{id}/market_references
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
  /rest/items/properties/{id}/market_references/{marketId}:
    delete:
      summary: Delete a property market reference
      description: Deletes a property market reference. The ID of the property and
        the ID of the market must be specified.
      operationId: deleteRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
    get:
      summary: Get a property market reference
      description: Gets a property market reference. The market ID and the property
        ID must be specified.
      operationId: getRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
    put:
      summary: Update a property market reference
      description: Updates a property market reference.
      operationId: putRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}/market_references/{marketId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
  /rest/items/properties/{id}/names:
    get:
      summary: List the property names
      description: Lists the names of a property in all languages. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesNames
      x-api-path-slug: restitemspropertiesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Names
    post:
      summary: Create a property name
      description: Creates a property name. The ID of the property must be specified.
      operationId: postRestItemsPropertiesNames
      x-api-path-slug: restitemspropertiesidnames-post
      parameters:
      - in: body
        name: /rest/items/properties/{id}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
  /rest/items/properties/{id}/names/{lang}:
    delete:
      summary: Delete a property name
      description: Deletes a property name. The ID of the property must be specified.
      operationId: deleteRestItemsPropertiesNamesLang
      x-api-path-slug: restitemspropertiesidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    get:
      summary: Get a property name
      description: Gets a property name in a specified language. The ID of the property
        and the language code must be specified.
      operationId: getRestItemsPropertiesNamesLang
      x-api-path-slug: restitemspropertiesidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    put:
      summary: Update a property name
      description: Updates a property name. The ID of the property and the language
        code must be specified.
      operationId: putRestItemsPropertiesNamesLang
      x-api-path-slug: restitemspropertiesidnameslang-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
  /rest/items/properties/{propertyId}/selections:
    get:
      summary: List property selections
      description: Lists the property selections of a property. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselections-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
    post:
      summary: Create a property selection
      description: Creates a property selection.
      operationId: postRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselections-post
      parameters:
      - in: body
        name: /rest/items/properties/{propertyId}/selections
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/items/properties/{propertyId}/selections/{id}:
    delete:
      summary: Delete a property selection
      description: Deletes a property selection. The ID of the property must be specified.
      operationId: deleteRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselectionsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    get:
      summary: Get a property selection
      description: Gets a property selection of a property.
      operationId: getRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselectionsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    post:
      summary: Creates a property selection lang
      description: Creates a property selection lang.
      operationId: postRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselectionsid-post
      parameters:
      - in: body
        name: /rest/items/properties/{propertyId}/selections/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Property
      - Selection
      - Lang
  /rest/items/properties/{propertyId}/selections/{id}/{lang}:
    delete:
      summary: Delete a property selection language
      description: Deletes a property selection language. The ID of the selection
        and the language must be specified.
      operationId: deleteRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
      - Language
    get:
      summary: List property selections by language
      description: Lists the property selections of a property for a specific language.
        The ID and language of the property must be specified.
      operationId: getRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
      - By
      - Language
    put:
      summary: Update a property selection
      description: Updates a property selection.
      operationId: putRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-put
      parameters:
      - in: body
        name: /rest/items/properties/{propertyId}/selections/{id}/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/items/properties/{propertyId}/selections/{lang}:
    get:
      summary: List property selections
      description: Lists the property selections of a property. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
  /rest/items/property_groups:
    get:
      summary: List property groups
      description: Lists the property groups.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-get
      parameters:
      - in: query
        name: with
        description: Includes the specified property group information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
    post:
      summary: Create a property group
      description: Creates a property group.
      operationId: postRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-post
      parameters:
      - in: body
        name: /rest/items/property_groups
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/items/property_groups/{id}:
    delete:
      summary: Delete a property group
      description: Deletes a property group. The ID of the property group must be
        specified.
      operationId: deleteRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    get:
      summary: Get a property group
      description: Gets a property group. The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    put:
      summary: Update a property group
      description: Updates an existing property group.
      operationId: putRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-put
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/items/property_groups/{id}/names:
    get:
      summary: List the property group names of a property group
      description: Lists the property group names of a property group in all languages.
        The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Group
      - Names
      - Of
      - Property
      - Group
    post:
      summary: Create a property group name
      description: Creates a property group name. The ID of the property group must
        be specified.
      operationId: postRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-post
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
  /rest/items/property_groups/{id}/names/{lang}:
    delete:
      summary: Delete a property group name
      description: Deletes a property group name. The ID of the property group must
        be specified.
      operationId: deleteRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
    get:
      summary: Get a property group name in a language
      description: Gets a property group name in the specified language. The ID of
        the property group name and the language code must be specified.
      operationId: getRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
      - In
      - Language
    put:
      summary: Update a property group name
      description: Updates a property group name. The ID of the property group and
        the language must be specified.
      operationId: putRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-put
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
  /rest/items/{id}/variations/{variationId}/variation_properties:
    delete:
      summary: Deletes all links between a variation and its property values
      description: Deletes all links between a variation and its property values.
        The ID of the variation must be specified.
      operationId: deleteRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Links
      - Between
      - Variation
      - Its
      - Property
      - Values
    get:
      summary: List property values linked to a variation
      description: Lists the property values linked to a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Values
      - Linked
      - To
      - Variation
    post:
      summary: Create link between variation and property value
      description: Creates a link between a variation and a property value.
      operationId: postRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Property
      - Value
  /rest/items/{id}/variations/{variationId}/variation_properties/{propertyId}:
    delete:
      summary: Delete link between variation and property value
      description: Delete a link between a variation and a property value. The ID
        of the item, the ID of the variation and the ID of the property must be specified.
      operationId: deleteRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Property
      - Value
    get:
      summary: Get a property value
      description: Gets a property value linked to a variation.
      operationId: getRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
    put:
      summary: Update a property value
      description: Update the data of a property value linked to a variation.
      operationId: putRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_properties/{propertyId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
  /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts:
    get:
      summary: Get property value texts
      description: Gets the texts saved for a specific property of the type Text in
        all available languages. The ID of the property must be specified.
      operationId: getRestItemsItemVariationsVariationVariationPropertiesPropertyTexts
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtexts-get
      parameters:
      - in: path
        name: itemId
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Texts
    post:
      summary: Create property value text by language
      description: Saves text for a specific property of the type Text in the specified
        language. The ID of the property and the language must be specified.
      operationId: postRestItemsItemVariationsVariationVariationPropertiesPropertyTexts
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtexts-post
      parameters:
      - in: body
        name: /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
  /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts/{lang}:
    delete:
      summary: Delete property value text by language
      description: Deletes the text saved for a specific property of the type Text
        in the specified language. The ID of the property  and the language must be
        specified.
      operationId: deleteRestItemsItemVariationsVariationVariationPropertiesPropertyTextsLang
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtextslang-delete
      parameters:
      - in: path
        name: itemId
      - in: path
        name: lang
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
    get:
      summary: Get property value text by language
      description: Gets the value text saved for a specific property of the type Text
        in the specified language. The ID of the property  and the language must be
        specified.
      operationId: getRestItemsItemVariationsVariationVariationPropertiesPropertyTextsLang
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtextslang-get
      parameters:
      - in: path
        name: itemId
      - in: path
        name: lang
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
    put:
      summary: Update property value text by language
      description: Updates the text saved for a specific property of the type Text
        in the specified language. The ID of the property and the language must be
        specified.
      operationId: putRestItemsItemVariationsVariationVariationPropertiesPropertyTextsLang
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtextslang-put
      parameters:
      - in: body
        name: /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      - in: path
        name: lang
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
  /rest/orders/items/properties:
    post:
      summary: Create an order item property.
      description: Create an order item property..
      operationId: postRestOrdersItemsProperties
      x-api-path-slug: restordersitemsproperties-post
      parameters:
      - in: body
        name: /rest/orders/items/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
  /rest/orders/items/properties/{id}:
    delete:
      summary: Delete an order item property by ID.
      description: Delete an order item property by id..
      operationId: deleteRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    get:
      summary: Get an order item property by ID.
      description: Get an order item property by id..
      operationId: getRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    put:
      summary: Update an order item property by ID.
      description: Update an order item property by id..
      operationId: putRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/items/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
  /rest/orders/items/{orderItemId}/properties/{typeId}:
    delete:
      summary: Delete an order item property by order item ID and order property type
        ID.
      description: Delete an order item property by order item id and order property
        type id..
      operationId: deleteRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    get:
      summary: Get an order item property by order item ID and order property type
        ID.
      description: Get an order item property by order item id and order property
        type id..
      operationId: getRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    post:
      summary: Create an order item property by order item ID and order property type
        ID.
      description: Create an order item property by order item id and order property
        type id..
      operationId: postRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    put:
      summary: Update an order item property by order item ID and order property type
        ID.
      description: Update an order item property by order item id and order property
        type id..
      operationId: putRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
  /rest/orders/properties/types:
    get:
      summary: List order property types
      description: Lists property types and their names in all languages. Optionally
        one or more languages can be specified to get a limited response.
      operationId: getRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-get
      parameters:
      - in: query
        name: lang
        description: Languages to be loaded with the type model
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Property
      - Types
    post:
      summary: Create an order property type
      description: Create an order property type.
      operationId: postRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-post
      parameters:
      - in: body
        name: /rest/orders/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Property
      - Type
  /rest/orders/properties/types/{typeId}:
    delete:
      summary: Delete a property type.
      description: Deletes a property type and all names for it from the database.
        The ID of the type must be specified.
      operationId: deleteRestOrdersPropertiesTypesType
      x-api-path-slug: restorderspropertiestypestypeid-delete
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
    get:
      summary: Get a property type
      description: Gets a property type and its names in all languages. Optionally
        one or more languages can be specified to get a limited response.
      operationId: getRestOrdersPropertiesTypesType
      x-api-path-slug: restorderspropertiestypestypeid-get
      parameters:
      - in: query
        name: lang
        description: Languages to be loaded with the type model
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
    put:
      summary: Update a property type.
      description: Updates a property type and its names. The ID of the type must
        be specified. You can also create new names, if you provide data which does
        not yet exist.
      operationId: putRestOrdersPropertiesTypesType
      x-api-path-slug: restorderspropertiestypestypeid-put
      parameters:
      - in: body
        name: /rest/orders/properties/types/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
  /rest/orders/properties/{id}:
    delete:
      summary: Delete a property of an order by property ID
      description: Deletes a property of an order. The ID of the property must be
        specified.
      operationId: deleteRestOrdersProperties
      x-api-path-slug: restorderspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Property
      - ID
    put:
      summary: Update a property of an order by property ID
      description: Updates the value of a property. The ID of the property must be
        specified.
      operationId: putRestOrdersProperties
      x-api-path-slug: restorderspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Property
      - ID
  /rest/orders/{orderId}/properties/{typeId}:
    delete:
      summary: Delete a property of an order by order ID and type ID
      description: Deletes a property of an order. The composite key of the property
        must be specified. The composite key is composed of the ID of the order and
        the ID of the order property type.
      operationId: deleteRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-delete
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Order
      - ID
      - Type
      - ID
    put:
      summary: Update a property of an order by order ID and property ID
      description: Updates the value of a property. The composite key of the property
        must be specified. The composite key is composed of the ID of the order and
        the ID of the order property type.
      operationId: putRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Order
      - ID
      - Property
      - ID
  /rest/payment/properties/types/names:
    post:
      summary: Create a name of a property type
      description: Create a name of a property type.
      operationId: postRestPaymentPropertiesTypesNames
      x-api-path-slug: restpaymentpropertiestypesnames-post
      parameters:
      - in: body
        name: /rest/payment/properties/types/names
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Property
      - Type
    put:
      summary: Update a name of a property type
      description: Update a name of a property type.
      operationId: putRestPaymentPropertiesTypesNames
      x-api-path-slug: restpaymentpropertiestypesnames-put
      parameters:
      - in: body
        name: /rest/payment/properties/types/names
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Property
      - Type
  /rest/payment/properties/types/names/{lang?}:
    get:
      summary: List names of property types
      description: List names of property types.
      operationId: getRestPaymentPropertiesTypesNamesLang
      x-api-path-slug: restpaymentpropertiestypesnameslang-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: lang?
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Property
      - Types
  /rest/payment/properties/types/names/{nameId}:
    get:
      summary: Get a name of a property type
      description: Gets a name of a property type. The ID of the name must be specified.
      operationId: getRestPaymentPropertiesTypesNamesName
      x-api-path-slug: restpaymentpropertiestypesnamesnameid-get
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Property
      - Type
  /rest/payments/properties/types:
    get:
      summary: List property types
      description: Lists all property types. The language must be specified.
      operationId: getRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Types
    post:
      summary: Create a property type
      description: Create a property type.
      operationId: postRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-post
      parameters:
      - in: body
        name: /rest/payments/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
    put:
      summary: Update a property type
      description: Update a property type.
      operationId: putRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-put
      parameters:
      - in: body
        name: /rest/payments/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
  /rest/payments/properties/types/{typeId}:
    get:
      summary: Get a property type
      description: Gets a property type. The ID of the type must be specified.
      operationId: getRestPaymentsPropertiesTypesType
      x-api-path-slug: restpaymentspropertiestypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
  /rest/payments/properties/{propertyId}:
    get:
      summary: Get a property
      description: Gets a property. The ID of the property must be specified.
      operationId: getRestPaymentsPropertiesProperty
      x-api-path-slug: restpaymentspropertiespropertyid-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/payments/property/{propertyTypeId}/{propertyValue}:
    get:
      summary: List payments by property type ID and value
      description: Lists all payments by the given property type ID and the value.
      operationId: getRestPaymentsPropertyPropertytypePropertyvalue
      x-api-path-slug: restpaymentspropertypropertytypeidpropertyvalue-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: propertyTypeId
      - in: path
        name: propertyValue
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Property
      - Type
      - ID
      - Value
  /rest/properties/destinations:
    get:
      summary: Get property destinations
      description: 'Returns a json with the destinations processed: data from providers
        and translations.'
      operationId: getRestPropertiesDestinations
      x-api-path-slug: restpropertiesdestinations-get
      responses:
        200:
          description: OK
      tags:
      - Property
      - Destinations
  /rest/properties/groups:
    get:
      summary: List property groups
      description: Lists property groups.
      operationId: getRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-get
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
    post:
      summary: Create a property group
      description: Creates a property group.
      operationId: postRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-post
      parameters:
      - in: body
        name: /rest/properties/groups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: names
        description: The names of the group
      - in: query
        name: options
        description: The options of the group
      - in: query
        name: position
        description: The position  of the group
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/groups/{groupId}:
    get:
      summary: Get a property group
      description: Gets a property group. The ID of the property group must be specified.
      operationId: getRestPropertiesGroupsGroup
      x-api-path-slug: restpropertiesgroupsgroupid-get
      parameters:
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    put:
      summary: Update a property group
      description: Updates a property group. The ID of the property group must be
        specified.
      operationId: putRestPropertiesGroupsGroup
      x-api-path-slug: restpropertiesgroupsgroupid-put
      parameters:
      - in: body
        name: /rest/properties/groups/{groupId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
      - in: query
        name: names
        description: The names of the group
      - in: query
        name: options
        description: The options of the group
      - in: query
        name: position
        description: The position  of the group
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/groups/{groupId}/properties/{propertyId}:
    delete:
      summary: Detach a property from a property group.
      description: Detaches a property from a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: deleteRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-delete
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Property
      - From
      - Property
      - Group
    post:
      summary: Attach a property to a property group
      description: Attaches a property to a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: postRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-post
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Attach
      - Property
      - To
      - Property
      - Group
  /rest/properties/groups/{propertyId}:
    delete:
      summary: Delete a property group
      description: Deletes a property group. The ID of the property group must be
        specified.
      operationId: deleteRestPropertiesGroupsProperty
      x-api-path-slug: restpropertiesgroupspropertyid-delete
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/markets:
    get:
      summary: List property markets
      description: Lists property markets
      operationId: getRestPropertiesMarkets
      x-api-path-slug: restpropertiesmarkets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Markets
    post:
      summary: Create a property market
      description: Creates a property market.
      operationId: postRestPropertiesMarkets
      x-api-path-slug: restpropertiesmarkets-post
      parameters:
      - in: body
        name: /rest/properties/markets
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: Property id
      - in: query
        name: referrerId
        description: The referrer id of the property market
      - in: query
        name: referrerSubId
        description: The referrer sub id of the property market
      - in: query
        name: value
        description: The value of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
  /rest/properties/markets/{propertiesMarketId}:
    delete:
      summary: Delete a property market
      description: Deletes a property market. The ID of the property market must be
        specified.
      operationId: deleteRestPropertiesMarketsPropertiesmarket
      x-api-path-slug: restpropertiesmarketspropertiesmarketid-delete
      parameters:
      - in: path
        name: propertiesMarketId
      - in: query
        name: propertyMarketId
        description: The ID of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
    get:
      summary: Get a property market
      description: Gets a property market. The ID of the property market must be specified.
      operationId: getRestPropertiesMarketsPropertiesmarket
      x-api-path-slug: restpropertiesmarketspropertiesmarketid-get
      parameters:
      - in: path
        name: propertiesMarketId
      - in: query
        name: propertyMarketId
        description: The ID of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
    put:
      summary: Update a property market
      description: Updates a property market. The ID of the property market must be
        specified.
      operationId: putRestPropertiesMarketsPropertiesmarket
      x-api-path-slug: restpropertiesmarketspropertiesmarketid-put
      parameters:
      - in: body
        name: /rest/properties/markets/{propertiesMarketId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: propertiesMarketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
  /rest/properties/names/{nameId}:
    delete:
      summary: Delete a property name
      description: Deletes a property name. The ID of the property name must be specified.
      operationId: deleteRestPropertiesNamesName
      x-api-path-slug: restpropertiesnamesnameid-delete
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    get:
      summary: Get a property name
      description: Gets a proeprty name. The ID of the property name must be specified.
      operationId: getRestPropertiesNamesName
      x-api-path-slug: restpropertiesnamesnameid-get
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    put:
      summary: Update a property name
      description: Updates a property name. The ID of the property name must be specified
      operationId: putRestPropertiesNamesName
      x-api-path-slug: restpropertiesnamesnameid-put
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
  /rest/properties/options:
    get:
      summary: List property options
      description: Lists property options.
      operationId: getRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Options
    post:
      summary: Create a property option
      description: Creates a property option.
      operationId: postRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-post
      parameters:
      - in: body
        name: /rest/properties/options
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: ID of the property
      - in: query
        name: typeOptionIdentifier
        description: The identifier of the property option type
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
  /rest/properties/options/{propertyOptionId}:
    delete:
      summary: Delete a property option
      description: Deletes a property option. The ID of the proeprty option must be
        specified.
      operationId: deleteRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-delete
      parameters:
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
    get:
      summary: Get a property option
      description: Gets a property option. The ID of the property option must be specified.
      operationId: getRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-get
      parameters:
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
    put:
      summary: Update a property option
      description: Updates a property option. The ID of the property option must be
        specified.
      operationId: putRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-put
      parameters:
      - in: query
        name: $propertyOptionId
        description: The ID of the property option
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
  /rest/properties/relations:
    delete:
      summary: Delete property relations
      description: Deletes property relations. The ID of the property relations must
        be specified.
      operationId: deleteRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-delete
      parameters:
      - in: query
        name: relationId
        description: The ID of the property relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relations
    get:
      summary: List property relations
      description: Lists property relations.
      operationId: getRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relations
    post:
      summary: Create a property relation
      description: Creates a property relation
      operationId: postRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-post
      parameters:
      - in: body
        name: /rest/properties/relations
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: relationTargetId
        description: The ID of the property relation target
      - in: query
        name: relationTypeIdentifier
        description: The identifier of the property relation type
      - in: query
        name: selectionRelationId
        description: The ID of the property selection relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
  /rest/properties/relations/markups:
    post:
      summary: Create a property relation markup
      description: Creates a property relation markup
      operationId: postRestPropertiesRelationsMarkups
      x-api-path-slug: restpropertiesrelationsmarkups-post
      parameters:
      - in: body
        name: /rest/properties/relations/markups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: markup
        description: The property relation markup
      - in: query
        name: propertyRelationId
        description: The ID of the property elation
      - in: query
        name: variationSalesPriceId
        description: The ID of a variations sales price
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
  /rest/properties/relations/markups/{relationMarkupId}:
    delete:
      summary: Delete a property relation markup
      description: Deletes a property relation markup
      operationId: deleteRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-delete
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
    get:
      summary: Get a property relation markup
      description: Gets a property relation markup. The ID of the property relation
        markup must be specified.
      operationId: getRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-get
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
    put:
      summary: Update a property relation markup
      description: Updates a property relation markup
      operationId: putRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-put
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
  /rest/properties/relations/values:
    get:
      summary: List property relation values
      description: Lists property relation values.
      operationId: getRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relation
      - Values
    post:
      summary: Create a property relation value
      description: Creates a property relation value.
      operationId: postRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-post
      parameters:
      - in: body
        name: /rest/properties/relations/values
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: lang
        description: The lang of the property relation value
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: value
        description: The value of the property relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
    put:
      summary: Update multiple property relation value
      description: Updates multiple property relation value
      operationId: putRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-put
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Property
      - Relation
      - Value
  /rest/properties/relations/values/{propertiesRelationValueId}:
    delete:
      summary: Delete a property relation value
      description: Deletes a property relation value. The ID of the property relation
        value must be specified.
      operationId: deleteRestPropertiesRelationsValuesPropertiesrelationvalue
      x-api-path-slug: restpropertiesrelationsvaluespropertiesrelationvalueid-delete
      parameters:
      - in: path
        name: propertiesRelationValueId
      - in: query
        name: propertyRelationValueId
        description: The ID of the property relation value
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
    put:
      summary: Update a property relation value
      description: Updates a property relation value. The ID of the property relation
        value must be specified.
      operationId: putRestPropertiesRelationsValuesPropertiesrelationvalue
      x-api-path-slug: restpropertiesrelationsvaluespropertiesrelationvalueid-put
      parameters:
      - in: query
        name: $propertyRelationValueId
        description: The ID of the property relation value
      - in: path
        name: propertiesRelationValueId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
  /rest/properties/relations/values/{relationMarkupId}:
    get:
      summary: Get a property relation value
      description: Gets a property relation value. The ID of the property relation
        value must be specified.
      operationId: getRestPropertiesRelationsValuesRelationmarkup
      x-api-path-slug: restpropertiesrelationsvaluesrelationmarkupid-get
      parameters:
      - in: query
        name: propertyRelationId
        description: The ID of the property relation
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
  /rest/properties/relations/{relationId}:
    delete:
      summary: Delete a property relation
      description: Deletes a property relation. The ID of the property relation must
        be specified.
      operationId: deleteRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-delete
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    get:
      summary: Get a property relation
      description: Gets a property relation. The ID of the property relation must
        be specified.
      operationId: getRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-get
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    put:
      summary: Update a property relation
      description: Updates a property relation. The ID of the property relation must
        be specified.
      operationId: putRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-put
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
  /rest/properties/selections:
    get:
      summary: List property selections
      description: Lists property selections
      operationId: getRestPropertiesSelections
      x-api-path-slug: restpropertiesselections-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
    post:
      summary: Create a property selection
      description: Creates a property selection.
      operationId: postRestPropertiesSelections
      x-api-path-slug: restpropertiesselections-post
      parameters:
      - in: body
        name: /rest/properties/selections
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: position
        description: The position of the property selection
      - in: query
        name: propertyId
        description: The ID of the property
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/properties/selections/{propertySelectionId}:
    delete:
      summary: Delete a property selection
      description: Deletes a property selection
      operationId: deleteRestPropertiesSelectionsPropertyselection
      x-api-path-slug: restpropertiesselectionspropertyselectionid-delete
      parameters:
      - in: path
        name: propertySelectionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    get:
      summary: Get a property selection
      description: Gets a property selection. The ID of property selection must be
        specified.
      operationId: getRestPropertiesSelectionsPropertyselection
      x-api-path-slug: restpropertiesselectionspropertyselectionid-get
      parameters:
      - in: path
        name: propertySelectionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    put:
      summary: Update a property selection
      description: Updates a property selection. The ID of the property selection
        must be specifed.
      operationId: putRestPropertiesSelectionsPropertyselection
      x-api-path-slug: restpropertiesselectionspropertyselectionid-put
      parameters:
      - in: query
        name: $propertySelectionId
        description: The ID of the property selection
      - in: path
        name: propertySelectionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/properties/{propertyId}:
    delete:
      summary: Delete a property
      description: Deletes a property. The ID of the property must be specified
      operationId: deleteRestPropertiesProperty
      x-api-path-slug: restpropertiespropertyid-delete
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
    get:
      summary: Get a property.
      description: Gets a property. The ID of the property must be specified.
      operationId: getRestPropertiesProperty
      x-api-path-slug: restpropertiespropertyid-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
    put:
      summary: Update a property
      description: Updates a property. The ID of the property must be specified.
      operationId: putRestPropertiesProperty
      x-api-path-slug: restpropertiespropertyid-put
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/storage/order-properties/object-url:
    get:
      summary: Get the URL for a order property file
      description: |-
        Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
        minutes.
      operationId: getRestStorageOrderPropertiesObjectUrl
      x-api-path-slug: reststorageorderpropertiesobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the order property     *                        file
          to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Order
      - Property
      - File
  /rest/orders/{orderId}/properties:
    post:
      summary: Create a property for an order
      description: Creates a property and attaches it to an order. The ID of the order
        must be specified.
      operationId: postRestOrdersOrderProperties
      x-api-path-slug: restordersorderidproperties-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Propertyan
      - Order
  /rest/properties/groups/{groupId}/properties:
    post:
      summary: Mass attach propertyId and groupId collection into the pivot table.
      description: Mass attach propertyid and groupid collection into the pivot table..
      operationId: postRestPropertiesGroupsGroupProperties
      x-api-path-slug: restpropertiesgroupsgroupidproperties-post
      parameters:
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Mass
      - Attach
      - PropertyId
      - GroupId
      - Collection
      - Into
      - Pivot
      - Table
  /rest/orders/items/{orderItemId}/properties:
    get:
      summary: Get all order item propertys for one order item by its order item id.
      description: Get all order item propertys for one order item by its order item
        id..
      operationId: getRestOrdersItemsOrderitemProperties
      x-api-path-slug: restordersitemsorderitemidproperties-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Propertysone
      - Order
      - Item
      - By
      - Its
      - Order
      - Item
      - Id
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