---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Lists favourited properties
  version: 1.0.0
  description: Lists favourited properties.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/auction/{id}/withdrawlots:
    post:
      summary: To withdraw a list of properties from the auction
      description: To withdraw a list of properties from the auction.
      operationId: Auction_WithdrawLotsByidBywithdrawLotsDataContract
      x-api-path-slug: apiauctionidwithdrawlots-post
      parameters:
      - in: path
        name: id
        description: The auction ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Withdraw
      - List
      - Of
      - Properties
      - From
      - Auction
  /api/documentgeneration/vendorreport:
    post:
      summary: Generates a correspondence to a single group, sending them a single
        report for multiple properties
      description: Generates a correspondence to a single group, sending them a single
        report for multiple properties.
      operationId: DocumentGeneration_SendVendorReportBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvendorreport-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Group
      - ""
      - Sending
      - Them
      - Single
      - Reportmultiple
      - Properties
  /api/documentgeneration/bulkpropertyownercommunication:
    post:
      summary: "Generates a bulk communication pack out to multiple vendors of properties.\r\nThis
        will ignore the target type set, as the document could only ever find the
        vendor as the contact item, so it always defaults\r\nto a target type of vendor/owner"
      description: "Generates a bulk communication pack out to multiple vendors of
        properties.\r\nthis will ignore the target type set, as the document could
        only ever find the vendor as the contact item, so it always defaults\r\nto
        a target type of vendor/owner."
      operationId: DocumentGeneration_BulkPropertyVendorCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkpropertyownercommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Vendors
      - Of
      - Properties
      - This
      - Will
      - Ignore
      - Target
      - Type
      - Set
      - ""
      - As
      - Document
      - Could
      - Only
      - Ever
      - Find
      - Vendor
      - As
      - Contact
      - Item
      - ""
      - So
      - It
      - Always
      - "Defaults\r\nTo"
      - Target
      - Type
      - Of
      - Vendor
      - Owner
  /api/documentgeneration/lettertemplate/properties/{id}:
    post:
      summary: Update the properties of a template, but not its content.
      description: Update the properties of a template, but not its content..
      operationId: DocumentGeneration_UpdateLetterTemplatePropertiesByidBytemplatePropertiesSaveDataContract
      x-api-path-slug: apidocumentgenerationlettertemplatepropertiesid-post
      parameters:
      - in: path
        name: id
        description: Document Id for the template
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: templatePropertiesSaveDataContract
        description: The letter template property changes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Properties
      - Of
      - Template
      - ""
      - But
      - Not
      - Its
      - Content
  /api/group/{id}/properties:
    get:
      summary: Return a list of properties that the group owns
      description: Return a list of properties that the group owns.
      operationId: Group_GroupPropertiesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidproperties-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Properties
      - That
      - Group
      - Owns
  /api/invoice/{id}/updatedetails:
    put:
      summary: Update properties on invoice
      description: Update properties on invoice.
      operationId: Invoice_UpdateInvoiceDetailsByidByupdateInvoiceDataContract
      x-api-path-slug: apiinvoiceidupdatedetails-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateInvoiceDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Properties
      - "On"
      - Invoice
  /api/negotiator/my/properties/{roleType}:
    get:
      summary: Used for the Property Sales Dashboard to return a list of the negotiator's
        properties.
      description: Used for the property sales dashboard to return a list of the negotiator's
        properties..
      operationId: Negotiator_PropertiesByroleTypeBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesroletype-get
      parameters:
      - in: query
        name: pageNumber
        description: which page number of results to choose
      - in: query
        name: pageSize
        description: how many properties to return (default 10)
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleType
        description: the PropertyMarketingRole type
      responses:
        200:
          description: OK
      tags:
      - Usedthe
      - Property
      - Sales
      - Dashboard
      - To
      - Return
      - List
      - Of
      - Negotiators
      - Properties
  /api/negotiator/my/properties/favourite:
    get:
      summary: Lists favourited properties
      description: Lists favourited properties.
      operationId: Negotiator_FavouritePropertiesBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesfavourite-get
      parameters:
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page Size
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Favourited
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