---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a csv file from selected letting property list items
  version: 1.0.0
  description: Generates a csv file from selected letting property list items.
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
  /api/property/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all properties
      description: Returns geoaggregations of all properties.
      operationId: Property_GeoAggregationByzoom
      x-api-path-slug: apipropertygeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Properties
  /api/role/auction/{id}/setrequestedlotnumber:
    post:
      summary: Set the requested lot number for a property auction role.
      description: Set the requested lot number for a property auction role..
      operationId: AuctionRole_SetRequestedLotNumberByidBylotNumber
      x-api-path-slug: apiroleauctionidsetrequestedlotnumber-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the requested lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Requested
      - Lot
      - Numbera
      - Property
      - Auction
      - Role
  /api/role/auction/{id}/setlotnumber:
    post:
      summary: Set the lot number for a property auction role.
      description: Set the lot number for a property auction role..
      operationId: AuctionRole_SetLotNumberByidByauctionIdBylotNumber
      x-api-path-slug: apiroleauctionidsetlotnumber-post
      parameters:
      - in: query
        name: auctionId
        description: the id of the auction to set the lot number for
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Lot
      - Numbera
      - Property
      - Auction
      - Role
  /api/role/auction/{id}/addtoauction:
    post:
      summary: Add a property auction role to an existing auction
      description: Add a property auction role to an existing auction.
      operationId: AuctionRole_AddToAuctionByidByauctionIdBylotNumber
      x-api-path-slug: apiroleauctionidaddtoauction-post
      parameters:
      - in: query
        name: auctionId
        description: the id of the auction to add the role to
      - in: path
        name: id
        description: the id of the role
      - in: query
        name: lotNumber
        description: the lot number
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - Auction
      - Role
      - To
      - Existing
      - Auction
  /api/role/auction/{id}/removefromauction:
    post:
      summary: Add a property auction role to an existing auction
      description: Add a property auction role to an existing auction.
      operationId: AuctionRole_RemoveFromAuctionByidByremoveFromAuctionDataContract
      x-api-path-slug: apiroleauctionidremovefromauction-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: body
        name: removeFromAuctionDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - Auction
      - Role
      - To
      - Existing
      - Auction
  /api/role/auction/{id}/setreserve:
    post:
      summary: Set the reserve for a property auction role.
      description: Set the reserve for a property auction role..
      operationId: AuctionRole_SetReserveByidBysetReserveDataContract
      x-api-path-slug: apiroleauctionidsetreserve-post
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setReserveDataContract
        description: SetReserveDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Reservea
      - Property
      - Auction
      - Role
  /api/customtextdescription/distinctcustompropertydescriptions:
    get:
      summary: Returns a list of the distinct defined custom descriptions for a property
      description: Returns a list of the distinct defined custom descriptions for
        a property.
      operationId: CustomTextDescription_DistinctCustomPropertyDescriptions
      x-api-path-slug: apicustomtextdescriptiondistinctcustompropertydescriptions-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Distinct
      - Defined
      - Custom
      - Descriptionsa
      - Property
  /api/todo/assignleadstoowningnegotiators:
    put:
      summary: Assign InboundLead Todos to the owning Negotiators of the property.
      description: Assign inboundlead todos to the owning negotiators of the property..
      operationId: DefaultToDo_AssignLeadsToOwningNegotiatorsBytoDoId
      x-api-path-slug: apitodoassignleadstoowningnegotiators-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - Assign
      - InboundLead
      - Todos
      - To
      - Owning
      - Negotiators
      - Of
      - Property
  /api/documentgeneration/previewpack:
    post:
      summary: Generates a pack using the first selected group/property of a type
        to get a quick preview of the pack
      description: Generates a pack using the first selected group/property of a type
        to get a quick preview of the pack.
      operationId: DocumentGeneration_PreviewPackByrandomPackDataContract
      x-api-path-slug: apidocumentgenerationpreviewpack-post
      parameters:
      - in: body
        name: randomPackDataContract
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
      - Pack
      - Using
      - First
      - Selected
      - Group
      - Property
      - Of
      - Type
      - To
      - Get
      - Quick
      - Preview
      - Of
      - Pack
  /api/documentgeneration/singlepropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same property role.
      operationId: DocumentGeneration_SendPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglepropertymatch-post
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
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Property
      - Role
  /api/documentgeneration/singlelettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same letting property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same letting property role.
      operationId: DocumentGeneration_SendLettingsPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglelettingspropertymatch-post
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
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Letting
      - Property
      - Role
  /api/documentgeneration/printablepropertylist:
    post:
      summary: Generates a printable property list, it is targetless so there is no
        reference to applicants or owners
      description: Generates a printable property list, it is targetless so there
        is no reference to applicants or owners.
      operationId: DocumentGeneration_PrintablePropertyListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationprintablepropertylist-post
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
      - Printable
      - Property
      - List
      - ""
      - It
      - Is
      - Targetless
      - So
      - There
      - Is
      - "No"
      - Reference
      - To
      - Applicants
      - Owners
  /api/documentgeneration/selectedpropertiesmatch:
    post:
      summary: Generates a correspondence to a single applicant, sending them user
        selected property roles
      description: Generates a correspondence to a single applicant, sending them
        user selected property roles.
      operationId: DocumentGeneration_SendSelectedPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedpropertiesmatch-post
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
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/selectedlettingspropertiesmatch:
    post:
      summary: Generates a correspondence to a single letting applicant, sending them
        user selected property roles
      description: Generates a correspondence to a single letting applicant, sending
        them user selected property roles.
      operationId: DocumentGeneration_SendSelectedLettingsPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedlettingspropertiesmatch-post
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
      - Letting
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/multipropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them a filtered
        set of the matching property roles
      description: Generates a correspondence to multiple applicants, sending them
        a filtered set of the matching property roles.
      operationId: DocumentGeneration_SendAutoMatchedPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultipropertymatch-post
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
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Property
      - Roles
  /api/documentgeneration/multilettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles
      description: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles.
      operationId: DocumentGeneration_SendAutoMatchedLettingsPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultilettingspropertymatch-post
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
      - Multiple
      - Letting
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Letting
      - Property
      - Roles
  /api/documentgeneration/recreatepropertymarketreport/{propertyId}:
    post:
      summary: Creates a new Property Market Report document.
      description: Creates a new property market report document..
      operationId: DocumentGeneration_RecreatePropertyMarketReportBypropertyId
      x-api-path-slug: apidocumentgenerationrecreatepropertymarketreportpropertyid-post
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Property
      - Market
      - Report
      - Document
  /api/event/recordpropertyownercontact:
    post:
      summary: Records an event on the role representing a neg being in contact for
        a property they own
      description: Records an event on the role representing a neg being in contact
        for a property they own.
      operationId: Event_RecordPropertyOwnerContactByrecordPropertyOwnerContactDataContract
      x-api-path-slug: apieventrecordpropertyownercontact-post
      parameters:
      - in: body
        name: recordPropertyOwnerContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contacta
      - Property
      - They
      - Own
  /api/event/addchatmessage:
    post:
      summary: Adds a message to the property
      description: Adds a message to the property.
      operationId: Event_AddChatMessageByaddChatMessageCommandDataContract
      x-api-path-slug: apieventaddchatmessage-post
      parameters:
      - in: body
        name: addChatMessageCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Message
      - To
      - Property
  /api/group/{id}/searching/{roleId}/matches:
    get:
      summary: Get property matches for a Searching Role for a Group
      description: Get property matches for a searching role for a group.
      operationId: Group_PropertyMatchesByidByroleIdBypageSizeBypageNumberBysort
      x-api-path-slug: apigroupidsearchingroleidmatches-get
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
      - in: path
        name: roleId
      - in: query
        name: sort
      responses:
        200:
          description: OK
      tags:
      - Property
      - Matchesa
      - Searching
      - Rolea
      - Group
    post:
      summary: Get property matches for a Searching Role for a Group
      description: Get property matches for a searching role for a group.
      operationId: Group_PropertyMatchesByidByroleIdByfilterBypageSizeBypageNumberBysort
      x-api-path-slug: apigroupidsearchingroleidmatches-post
      parameters:
      - in: body
        name: filter
        description: Match filter
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Group Id
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Amount of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: Role Id
      - in: query
        name: sort
        description: How to sort the results
      responses:
        200:
          description: OK
      tags:
      - Property
      - Matchesa
      - Searching
      - Rolea
      - Group
  /api/group/matches/find:
    post:
      summary: Returns property matches using their Id
      description: Returns property matches using their id.
      operationId: Group_FindMatchesByqueryDataContract
      x-api-path-slug: apigroupmatchesfind-post
      parameters:
      - in: body
        name: queryDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Matches
      - Using
      - Their
      - Id
  /api/group/{id}/getpropertyroleidsalreadysent:
    get:
      summary: returns a list of the property role ids that should be excluded from
        mailouts to this role id because the have been sent before
      description: Returns a list of the property role ids that should be excluded
        from mailouts to this role id because the have been sent before.
      operationId: Group_GetPropertyMarketingRoleIdsSentByidBywithinDaysByresendPriceChangedProperties
      x-api-path-slug: apigroupidgetpropertyroleidsalreadysent-get
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: query
        name: resendPriceChangedProperties
        description: include the properties that have had to a price change or withdrawn
          event since it was last sent to them
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: withinDays
        description: number of days since the last time it was sent, send 0 for all
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Property
      - Role
      - Ids
      - That
      - Should
      - Be
      - Excluded
      - From
      - Mailouts
      - To
      - This
      - Role
      - Id
      - Because
      - Have
      - Been
      - Sent
      - Before
  /api/property/{id}/historicalprices:
    get:
      summary: Get historical prices for a property by its Id
      description: Get historical prices for a property by its id.
      operationId: HistoricalPrice_GetByPropertyIdByidBypageNumberBypageSize
      x-api-path-slug: apipropertyidhistoricalprices-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get
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
      - Historical
      - Pricesa
      - Property
      - By
      - Its
      - Id
  /api/property/historicalprices/postcode/{postcode}:
    get:
      summary: Get historical prices for a property by its Id
      description: Get historical prices for a property by its id.
      operationId: HistoricalPrice_GetByPostcodeBypostcodeBypropertyTypeBystyleTypeByleaseTypeBypageNumberBypageSize
      x-api-path-slug: apipropertyhistoricalpricespostcodepostcode-get
      parameters:
      - in: query
        name: leaseType
        description: 'Options are: Freehold, Leasehold'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: path
        name: postcode
        description: The postcode to get historical price data for
      - in: query
        name: propertyType
        description: 'Options are: DetachedHouse, SemiDetachedHouse, TerracedHouse,
          Flat'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: styleType
        description: 'Options are: New, Older'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Pricesa
      - Property
      - By
      - Its
      - Id
  /api/list/property/filters/{id}:
    delete:
      summary: Marks Property List Filter as deleted
      description: Marks property list filter as deleted.
      operationId: List_DeletePropertyFilterByid
      x-api-path-slug: apilistpropertyfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Property
      - List
      - Filter
      - As
      - Deleted
  /api/list/property/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
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
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/lettingproperty/csv:
    post:
      summary: Generates a csv file from selected letting property list items
      description: Generates a csv file from selected letting property list items.
      operationId: List_GenerateLettingPropertyCsvBycommandDataContract
      x-api-path-slug: apilistlettingpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
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
      - Csv
      - File
      - From
      - Selected
      - Letting
      - Property
      - List
      - Items
  /api/list/propertypipeline/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePipelinePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertypipelinecsv-post
      parameters:
      - in: body
        name: commandDataContract
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
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/groupmatches/csv:
    post:
      summary: Generates a csv file from group matches by property role id
      description: Generates a csv file from group matches by property role id.
      operationId: List_GenerateGroupMatchesCsvBycommandDataContract
      x-api-path-slug: apilistgroupmatchescsv-post
      parameters:
      - in: body
        name: commandDataContract
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
      - Csv
      - File
      - From
      - Group
      - Matches
      - By
      - Property
      - Role
      - Id
  /api/list/propertynewbusiness/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GenerateNewBusinessPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertynewbusinesscsv-post
      parameters:
      - in: body
        name: commandDataContract
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
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/negotiator/my/properties/favourite/add/{propertyId}:
    post:
      summary: Add property to Negotiators favourite list
      description: Add property to negotiators favourite list.
      operationId: Negotiator_AddFavouritePropertyBypropertyIdByroleId
      x-api-path-slug: apinegotiatormypropertiesfavouriteaddpropertyid-post
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Property
      - To
      - Negotiators
      - Favourite
      - List
  /api/negotiator/my/properties/favourite/remove/{propertyId}:
    delete:
      summary: Remove a property from a Negotiators favourite list.
      description: Remove a property from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouritePropertyBypropertyIdByroleId
      x-api-path-slug: apinegotiatormypropertiesfavouriteremovepropertyid-delete
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Property
      - From
      - Negotiators
      - Favourite
      - List
  /api/admin/portal/getportaluploadsforrole:
    get:
      summary: Get all the live portal uploads associated with a property marketing
        role
      description: Get all the live portal uploads associated with a property marketing
        role.
      operationId: Portal_GetLivePortalInformationRecordsForRoleByroleId
      x-api-path-slug: apiadminportalgetportaluploadsforrole-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Live
      - Portal
      - Uploads
      - Associated
      - Property
      - Marketing
      - Role
  /api/progression/withdrawinstruction:
    put:
      summary: Add withdrawalvaluation to a property sales role
      description: Add withdrawalvaluation to a property sales role.
      operationId: Progression_WithdrawInstructionBywithdrawInstructionDataContract
      x-api-path-slug: apiprogressionwithdrawinstruction-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawInstructionDataContract
        description: Details of the progression withdrawal
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Withdrawalvaluation
      - To
      - Property
      - Sales
      - Role
  /api/progression/withdrawvaluation:
    put:
      summary: Add WithdrawVal to a property sales role
      description: Add withdrawval to a property sales role.
      operationId: Progression_WithdrawValuationBywithdrawValuationDataContract
      x-api-path-slug: apiprogressionwithdrawvaluation-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawValuationDataContract
        description: Details of the progression withdrawal
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - WithdrawVal
      - To
      - Property
      - Sales
      - Role
  /api/property/{id}:
    get:
      summary: Get a property by its Id
      description: Get a property by its id.
      operationId: Property_GetByid
      x-api-path-slug: apipropertyid-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Property
      - By
      - Its
      - Id
  /api/property/{id}/updateaddress:
    put:
      summary: A command driven endpoint to Update a property address.
      description: A command driven endpoint to update a property address..
      operationId: Property_UpdateAddressByidByaddressDataContract
      x-api-path-slug: apipropertyidupdateaddress-put
      parameters:
      - in: body
        name: addressDataContract
        description: The address data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - ""
      - Property
      - Address
  /api/property/{id}/owners/events:
    get:
      summary: Get property events for the current owner by its Id
      description: Get property events for the current owner by its id.
      operationId: Property_OwnersEventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryType
      x-api-path-slug: apipropertyidownersevents-get
      parameters:
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the property to get events for
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Property
      - Eventsthe
      - Current
      - Owner
      - By
      - Its
      - Id
  /api/property/{id}/events:
    get:
      summary: Get property events by its Id
      description: Get property events by its id.
      operationId: Property_EventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryType
      x-api-path-slug: apipropertyidevents-get
      parameters:
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the property to get events for
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Property
      - Events
      - By
      - Its
      - Id
  /api/property/{id}/descriptions:
    get:
      summary: Get the descriptions for a property by property id
      description: Get the descriptions for a property by property id.
      operationId: Property_DescriptionsByidBypageSizeBypageNumberBytypes
      x-api-path-slug: apipropertyiddescriptions-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get the descriptions for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: types
      responses:
        200:
          description: OK
      tags:
      - Descriptionsa
      - Property
      - By
      - Property
      - Id
  /api/property/{id}/roles:
    get:
      summary: Get the roles for a property by property id
      description: Get the roles for a property by property id.
      operationId: Property_RolesByidBypageSizeBypageNumberByroleTypesByroleStatuses
      x-api-path-slug: apipropertyidroles-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get the roles for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleStatuses
      - in: query
        name: roleTypes
      responses:
        200:
          description: OK
      tags:
      - Rolesa
      - Property
      - By
      - Property
      - Id
  /api/property/{id}/documents:
    get:
      summary: Get the documents of a property by the property Id
      description: Get the documents of a property by the property id.
      operationId: Property_DocumentsByidBysubTypesBypageSizeBypageNumberBytype
      x-api-path-slug: apipropertyiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Of
      - Property
      - By
      - Property
      - Id
  /api/property/comparables:
    get:
      summary: For a given property, will return all comparable property's nearby.
      description: For a given property, will return all comparable property's nearby..
      operationId: Property_ComparablesBypropertyIdBylatitudeBylongitudeBymileRadiusBypageSizeBypageNumberBybranchIdByi
      x-api-path-slug: apipropertycomparables-get
      parameters:
      - in: query
        name: branchId
        description: Optional Branch Id
      - in: query
        name: isForLetting
        description: Indicate if the request is for Sales or Lettings
      - in: query
        name: latitude
        description: The latitude to find comparables for
      - in: query
        name: longitude
        description: The longitude to find comparables for
      - in: query
        name: mileRadius
        description: how near to compare (default 1 mile)
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: query
        name: propertyId
        description: The id of the property to find comparables for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - For
      - Given
      - Property
      - ""
      - Will
      - Return
      - ""
      - Comparable
      - Propertys
      - Nearby
  /api/property/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a property
      description: Attaches an existing document to a property.
      operationId: Property_AttachDocumentByidBydocumentId
      x-api-path-slug: apipropertyidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the property to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Property
  /api/property/{id}/detachdocument:
    put:
      summary: Detaches a document from a property
      description: Detaches a document from a property.
      operationId: Property_DetachDocumentByidBydocumentId
      x-api-path-slug: apipropertyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the property description to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Property
  /api/property/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a property.
      description: Allows you to upload a document and attach it directly to a property..
      operationId: Property_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apipropertyiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Details o
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Property
  /api/property/{id}/attachexternaldocument:
    post:
      summary: Attaches an externally hosted document to a property
      description: Attaches an externally hosted document to a property.
      operationId: Property_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apipropertyidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: Details of the document to associate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Property
  /api/property/{id}/valuations:
    get:
      summary: Get all of the valuations associated to the current owner of the property.
      description: Get all of the valuations associated to the current owner of the
        property..
      operationId: Property_ValuationsByidBypageSizeBypageNumber
      x-api-path-slug: apipropertyidvaluations-get
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
      - Of
      - Valuations
      - Associated
      - To
      - Current
      - Owner
      - Of
      - Property
  /api/property/{id}/valued:
    get:
      summary: Get all of the valued for current owner of the property.
      description: Get all of the valued for current owner of the property..
      operationId: Property_ValuedByidBypageSizeBypageNumber
      x-api-path-slug: apipropertyidvalued-get
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
      - Of
      - Valuedcurrent
      - Owner
      - Of
      - Property
  /api/property/{id}/owners:
    get:
      summary: For a given property, will return owning PeopleGroup
      description: For a given property, will return owning peoplegroup.
      operationId: Property_OwnersByid
      x-api-path-slug: apipropertyidowners-get
      parameters:
      - in: path
        name: id
        description: property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - For
      - Given
      - Property
      - ""
      - Will
      - Return
      - Owning
      - PeopleGroup
  /api/property/{id}/keys:
    get:
      summary: Get a list of keys for a property
      description: Get a list of keys for a property.
      operationId: Property_KeysByid
      x-api-path-slug: apipropertyidkeys-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Keysa
      - Property
  /api/property/{id}/alarms:
    get:
      summary: Get a list of alarms for a property
      description: Get a list of alarms for a property.
      operationId: Property_AlarmsByid
      x-api-path-slug: apipropertyidalarms-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Alarmsa
      - Property
  /api/property/{id}/specialarrangements:
    get:
      summary: Get a list of special arrangements for a property
      description: Get a list of special arrangements for a property.
      operationId: Property_SpecialArrangementsByid
      x-api-path-slug: apipropertyidspecialarrangements-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Special
      - Arrangementsa
      - Property
  /api/property/{id}/keys/add:
    post:
      summary: Add keys for a property
      description: Add keys for a property.
      operationId: Property_AddKeysByidBykeysToAdd
      x-api-path-slug: apipropertyidkeysadd-post
      parameters:
      - in: path
        name: id
        description: The property id
      - in: body
        name: keysToAdd
        description: A collection of keys to add
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Keysa
      - Property
  /api/property/{id}/alarms/add:
    post:
      summary: Add alarm codes for a property
      description: Add alarm codes for a property.
      operationId: Property_AddAlarmsByidByalarmsToAdd
      x-api-path-slug: apipropertyidalarmsadd-post
      parameters:
      - in: body
        name: alarmsToAdd
        description: A collection of alarm codes to add
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Alarm
      - Codesa
      - Property
  /api/property/{id}/specialarrangements/add:
    post:
      summary: Add special arrangements for a property
      description: Add special arrangements for a property.
      operationId: Property_AddSpecialArrangementsByidByarrangementsToAdd
      x-api-path-slug: apipropertyidspecialarrangementsadd-post
      parameters:
      - in: body
        name: arrangementsToAdd
        description: A collection of arrangements codes to add
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Special
      - Arrangementsa
      - Property
  /api/property/{id}/keys/remove:
    delete:
      summary: Remove keys from a property
      description: Remove keys from a property.
      operationId: Property_RemoveKeysByidBykeyIds
      x-api-path-slug: apipropertyidkeysremove-delete
      parameters:
      - in: path
        name: id
        description: The property id
      - in: query
        name: keyIds
        description: The ids of the keys to remove
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Keys
      - From
      - Property
  /api/property/{id}/alarms/remove:
    delete:
      summary: Remove alarm codes from a property
      description: Remove alarm codes from a property.
      operationId: Property_RemoveAlarmsByidByalarmIds
      x-api-path-slug: apipropertyidalarmsremove-delete
      parameters:
      - in: query
        name: alarmIds
        description: The ids of the alarm codes to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Alarm
      - Codes
      - From
      - Property
  /api/property/{id}/specialarrangements/remove:
    delete:
      summary: Remove special arrangements from a property
      description: Remove special arrangements from a property.
      operationId: Property_RemoveSpecialArrangementsByidByarrangementIds
      x-api-path-slug: apipropertyidspecialarrangementsremove-delete
      parameters:
      - in: query
        name: arrangementIds
        description: The ids of the special arrangements to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Special
      - Arrangements
      - From
      - Property
  /api/property/{id}/keys/checkout:
    put:
      summary: Checkout a collection of keys for a property
      description: Checkout a collection of keys for a property.
      operationId: Property_CheckoutKeysByidBycheckoutDetails
      x-api-path-slug: apipropertyidkeyscheckout-put
      parameters:
      - in: body
        name: checkoutDetails
        description: The details of the keys to checkout
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Collection
      - Of
      - Keysa
      - Property
  /api/property/{id}/keys/checkin:
    put:
      summary: Checkin a collection of keys for a property
      description: Checkin a collection of keys for a property.
      operationId: Property_CheckinKeysByidBycheckinDetails
      x-api-path-slug: apipropertyidkeyscheckin-put
      parameters:
      - in: body
        name: checkinDetails
        description: The details of the keys to checkin
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Collection
      - Of
      - Keysa
      - Property
  /api/property/{id}/certificate:
    get:
      summary: Get a list of certificates for a property
      description: Get a list of certificates for a property.
      operationId: Property_CertificateByid
      x-api-path-slug: apipropertyidcertificate-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Certificatesa
      - Property
  /api/property/{id}/certificate/add:
    post:
      summary: Add certificate for a property
      description: Add certificate for a property.
      operationId: Property_AddCertificateByidBycertificateToAdd
      x-api-path-slug: apipropertyidcertificateadd-post
      parameters:
      - in: body
        name: certificateToAdd
        description: A certificate to add
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Certificatea
      - Property
  /api/property/{id}/certificate/remove:
    delete:
      summary: Remove certificate from a property
      description: Remove certificate from a property.
      operationId: Property_RemoveCertificateByidBycertificateId
      x-api-path-slug: apipropertyidcertificateremove-delete
      parameters:
      - in: query
        name: certificateId
        description: The ids of the certificate to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Certificate
      - From
      - Property
  /api/property/{id}/tenantroles:
    get:
      summary: Get a list of all current and ended tenant roles from a property id.
      description: Get a list of all current and ended tenant roles from a property
        id..
      operationId: Property_TenantRolesByPropertyIdByid
      x-api-path-slug: apipropertyidtenantroles-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Current
      - Ended
      - Tenant
      - Roles
      - From
      - Property
      - Id
  /api/todo/property/savetodo:
    post:
      summary: Save or Updates a Property ToDo and and its tasks
      description: Save or updates a property todo and and its tasks.
      operationId: PropertyToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodopropertysavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - S
      - Property
      - ToDo
      - And
      - Its
      - Tasks
  /api/todo/property/addtasks:
    put:
      summary: Add tasks to a Property ToDo
      description: Add tasks to a property todo.
      operationId: PropertyToDo_AddTasksByaddPropertyTasksCommandDataContract
      x-api-path-slug: apitodopropertyaddtasks-put
      parameters:
      - in: body
        name: addPropertyTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - To
      - Property
      - ToDo
  /api/role/{id}/matches:
    get:
      summary: Get a list of groups that may be interested in this property role
      description: Get a list of groups that may be interested in this property role.
      operationId: Role_MatchesByidBypageSizeBypageNumberByadjustedAskingPriceBysortByminScore
      x-api-path-slug: apiroleidmatches-get
      parameters:
      - in: query
        name: adjustedAskingPrice
        description: Override the asking price to show a different set of potential
          matches
      - in: path
        name: id
        description: The id of the role to get the group matches for
      - in: query
        name: minScore
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Number of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: sort
        description: Sort order of results
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - That
      - May
      - Be
      - Interested
      - In
      - This
      - Property
      - Role
    post:
      summary: Get a list of groups that may be interested in this property role
      description: Get a list of groups that may be interested in this property role.
      operationId: Role_MatchesByidByfilterBypageSizeBypageNumberByadjustedAskingPriceBysort
      x-api-path-slug: apiroleidmatches-post
      parameters:
      - in: query
        name: adjustedAskingPrice
        description: Override the asking price to show a different set of potential
          matches
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the role to get the group matches for
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Number of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: sort
        description: Sort order of results
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - That
      - May
      - Be
      - Interested
      - In
      - This
      - Property
      - Role
  /api/role/{id}/valuation:
    get:
      summary: Gets the valuation for a property marketing role
      description: Gets the valuation for a property marketing role.
      operationId: Role_GetValuationByid
      x-api-path-slug: apiroleidvaluation-get
      parameters:
      - in: path
        name: id
        description: The id of the property marketing role to find a valuation for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Valuationa
      - Property
      - Marketing
      - Role
  /api/role/{id}/valued:
    get:
      summary: Gets the valuation for a property marketing role
      description: Gets the valuation for a property marketing role.
      operationId: Role_GetValuedByid
      x-api-path-slug: apiroleidvalued-get
      parameters:
      - in: path
        name: id
        description: The id of the property marketing role to find a valuation for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Valuationa
      - Property
      - Marketing
      - Role
  /api/role/{id}/offers:
    get:
      summary: Get all of the offers associated to the current property marketing
        role.
      description: Get all of the offers associated to the current property marketing
        role..
      operationId: Role_OffersByidBypageSizeBypageNumberByexcludeDrafts
      x-api-path-slug: apiroleidoffers-get
      parameters:
      - in: query
        name: excludeDrafts
      - in: path
        name: id
        description: The id of the role to get the offers for
      - in: query
        name: pageNumber
        description: Page number to return
      - in: query
        name: pageSize
        description: Page size to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Of
      - Offers
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{id}/offersbasic:
    get:
      summary: Get a basic list of offers associated to the current property marketing
        role.
      description: Get a basic list of offers associated to the current property marketing
        role..
      operationId: Role_OffersBasicByid
      x-api-path-slug: apiroleidoffersbasic-get
      parameters:
      - in: path
        name: id
        description: The id of the marketing role to get the offers for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Basic
      - List
      - Of
      - Offers
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{id}/viewings:
    get:
      summary: Get all of the viewings associated to the current property marketing
        role.
      description: Get all of the viewings associated to the current property marketing
        role..
      operationId: Role_ViewingsByidBypageSizeBypageNumberByexcludeDrafts
      x-api-path-slug: apiroleidviewings-get
      parameters:
      - in: query
        name: excludeDrafts
      - in: path
        name: id
        description: The id of the role to get the offers for
      - in: query
        name: pageNumber
        description: Page number to return
      - in: query
        name: pageSize
        description: Page size to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Of
      - Viewings
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{id}/setdefaultimage:
    put:
      summary: Sets the default image of a property marketing role
      description: Sets the default image of a property marketing role.
      operationId: Role_SetDefaultImageByidBydocumentId
      x-api-path-slug: apiroleidsetdefaultimage-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to set as the default image
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Default
      - Image
      - Of
      - Property
      - Marketing
      - Role
  /api/role/{id}/setflag:
    put:
      summary: Sets a flag on a property marketing role
      description: Sets a flag on a property marketing role.
      operationId: Role_SetFlagByidBysetMarketingFlagDataContract
      x-api-path-slug: apiroleidsetflag-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setMarketingFlagDataContract
        description: The flag detail
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Flag
      - "On"
      - Property
      - Marketing
      - Role
  /api/role/{id}/setcompliancechecks:
    put:
      summary: Set the compliance checks on a property marketing role i.e. Valid Epc,
        Proof of ID or Proof of Ownership.
      description: Set the compliance checks on a property marketing role i.e. valid
        epc, proof of id or proof of ownership..
      operationId: Role_SetComplianceChecksByidBysetComplianceChecksDataContract
      x-api-path-slug: apiroleidsetcompliancechecks-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setComplianceChecksDataContract
        description: The flag detail
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Compliance
      - Checks
      - "On"
      - Property
      - Marketing
      - Role
      - I
      - E
      - ""
      - Valid
      - Epc
      - ""
      - Proof
      - Of
      - ID
      - Proof
      - Of
      - Ownership
  /api/role/{id}/copy:
    post:
      summary: Clones a property marketing role
      description: Clones a property marketing role.
      operationId: Role_CopySalesMarketingRoleByid
      x-api-path-slug: apiroleidcopy-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Clones
      - Property
      - Marketing
      - Role
  /api/simplepropertyrole/{roleId}:
    get:
      summary: Get a property with an associated role by their Id's
      description: Get a property with an associated role by their id's.
      operationId: SimplePropertyRole_GetByroleId
      x-api-path-slug: apisimplepropertyroleroleid-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The role Id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Associated
      - Role
      - By
      - Their
      - Ids
  /api/admin/system/sendliveportalupdatemessage:
    post:
      summary: "Sends a message to the LivePortalJobHandler that says \r\nthe specified
        property marketing role has changed"
      description: "Sends a message to the liveportaljobhandler that says \r\nthe
        specified property marketing role has changed."
      operationId: System_SendLivePortalUpdateMessageBypropertyMarketingRoleId
      x-api-path-slug: apiadminsystemsendliveportalupdatemessage-post
      parameters:
      - in: query
        name: propertyMarketingRoleId
        description: The property marketing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Message
      - To
      - LivePortalJobHandler
      - That
      - Says
      - The
      - Specified
      - Property
      - Marketing
      - Role
      - Has
      - Changed
  /api/property/{id}/addgrouptoproperty:
    put:
      summary: Creates/Adds a group to the CurrentOwners of the supplied PropertyId
      description: Creates/adds a group to the currentowners of the supplied propertyid.
      operationId: Property_AddGroupToPropertyByidBydatacontract
      x-api-path-slug: apipropertyidaddgrouptoproperty-put
      parameters:
      - in: body
        name: datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Group
      - To
      - CurrentOwners
      - Of
      - Supplied
      - PropertyId
  /api/role/lettings/{id}/setrentshare:
    put:
      summary: Set the rent share for landlords on PropertyLettingRole
      description: Set the rent share for landlords on propertylettingrole.
      operationId: LettingRole_SetRentShareByidByshareDataContracts
      x-api-path-slug: apirolelettingsidsetrentshare-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: shareDataContracts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Rent
      - Sharelandlords
      - "On"
      - PropertyLettingRole
  /api/role/lettings/{id}/settobsigned:
    put:
      summary: Set the terms of business for a landlord on a PropertyLettingRole
      description: Set the terms of business for a landlord on a propertylettingrole.
      operationId: LettingRole_SetTOBSignedByidBydataContract
      x-api-path-slug: apirolelettingsidsettobsigned-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Terms
      - Of
      - Businessa
      - Landlord
      - "On"
      - PropertyLettingRole
  /api/role/lettings/{id}/setnrldetails:
    put:
      summary: Set the NRL details for a landlord on a PropertyLettingRole
      description: Set the nrl details for a landlord on a propertylettingrole.
      operationId: LettingRole_SetNRLDetailsByidBydataContract
      x-api-path-slug: apirolelettingsidsetnrldetails-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - NRL
      - Detailsa
      - Landlord
      - "On"
      - PropertyLettingRole
  /api/progression/lettings/remarket:
    post:
      summary: Remarket a Letting. Completes the PropertyLettingRole and the TenantRole
        and creates a new PropertyLettingRole
      description: Remarket a letting. completes the propertylettingrole and the tenantrole
        and creates a new propertylettingrole.
      operationId: LettingsProgression_RemarketByremarketCommandDataContract
      x-api-path-slug: apiprogressionlettingsremarket-post
      parameters:
      - in: body
        name: remarketCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remarket
      - Letting
      - ""
      - Completes
      - PropertyLettingRole
      - TenantRole
      - Creates
      - New
      - PropertyLettingRole
  /api/role/{id}/updatefees:
    put:
      summary: Update the fee for a given PropertyMarketingRole.
      description: Update the fee for a given propertymarketingrole..
      operationId: Role_UpdateFeesByidByfeeDataContracts
      x-api-path-slug: apiroleidupdatefees-put
      parameters:
      - in: body
        name: feeDataContracts
        description: The fees to apply to the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feea
      - Given
      - PropertyMarketingRole
  /api/role/{id}/addfee:
    put:
      summary: Add a fee for a given PropertyMarketingRole.
      description: Add a fee for a given propertymarketingrole..
      operationId: Role_AddFeeByidByfeeDataContract
      x-api-path-slug: apiroleidaddfee-put
      parameters:
      - in: body
        name: feeDataContract
        description: The fee to add to the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feea
      - Given
      - PropertyMarketingRole
  /api/role/{id}/removefee:
    put:
      summary: Remove a fee from a given PropertyMarketingRole.
      description: Remove a fee from a given propertymarketingrole..
      operationId: Role_RemoveFeeByidByfeeId
      x-api-path-slug: apiroleidremovefee-put
      parameters:
      - in: query
        name: feeId
        description: The Id of the fee to remove
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Given
      - PropertyMarketingRole
  /api/roomdescription/{id}/attachtorole:
    put:
      summary: Attach a RoomDescription to a PropertyMarketingRole
      description: Attach a roomdescription to a propertymarketingrole.
      operationId: RoomDescription_AttachToRoleByidByroleId
      x-api-path-slug: apiroomdescriptionidattachtorole-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Attach
      - RoomDescription
      - To
      - PropertyMarketingRole
  /api/role/sales/{id}/getepc:
    get:
      summary: Gets EPC from the supplied propertyRoleId
      description: Gets epc from the supplied propertyroleid.
      operationId: SalesRole_GetEPCByid
      x-api-path-slug: apirolesalesidgetepc-get
      parameters:
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - EPC
      - From
      - Supplied
      - PropertyRoleId
  /api/role/sales/{id}/saveepc:
    post:
      summary: Creates/Overrides the EPC for the supplied propertyRoleId
      description: Creates/overrides the epc for the supplied propertyroleid.
      operationId: SalesRole_SaveEPCByidBydatacontract
      x-api-path-slug: apirolesalesidsaveepc-post
      parameters:
      - in: body
        name: datacontract
        description: The EPC information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Overrides
      - EPCthe
      - Supplied
      - PropertyRoleId
  /api/role/{id}/updateprice:
    put:
      summary: Update price for a given PropertySalesRole.
      description: Update price for a given propertysalesrole..
      operationId: Role_UpdatePriceByidByupdatePriceDataContract
      x-api-path-slug: apiroleidupdateprice-put
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updatePriceDataContract
        description: UpdatePriceDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Pricea
      - Given
      - PropertySalesRole
  /api/todo/property/taskprofile:
    get:
      summary: Get the profile infos for a propery task
      description: Get the profile infos for a propery task.
      operationId: PropertyToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodopropertytaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Propery
      - Task
  /api/globalsearch/properties:
    get:
      summary: Search for Properties across the system.
      description: Search for properties across the system..
      operationId: GlobalSearch_PropertiesBydataContract.termBydataContract.pageSizeBydataContract.pageNumberBydataCont
      x-api-path-slug: apiglobalsearchproperties-get
      parameters:
      - in: query
        name: dataContract.branchId
      - in: query
        name: dataContract.excludeArchived
      - in: query
        name: dataContract.excludeDeleted
      - in: query
        name: dataContract.groupTypes
      - in: query
        name: dataContract.lastUpdated
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.serviceType
      - in: query
        name: dataContract.term
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - SearchProperties
      - Across
      - System
  /api/role/lettings/{id}/setheadlandlord:
    put:
      summary: Set the head landlord for PropertyLettingRole
      description: Set the head landlord for propertylettingrole.
      operationId: LettingRole_SetHeadLandlordByidBypersonIdBygroupId
      x-api-path-slug: apirolelettingsidsetheadlandlord-put
      parameters:
      - in: query
        name: groupId
      - in: path
        name: id
      - in: query
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Head
      - LandlordPropertyLettingRole
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