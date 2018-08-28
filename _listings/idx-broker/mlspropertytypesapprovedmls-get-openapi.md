---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Get Mls Propertytypes Approvedmls
  description: Gives the property type information for all types that are available
    on a given MLS.
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
  /clients/properties/{savedLinkId}:
    get:
      summary: Get Properties Saved Link
      description: Get client saved links results
      operationId: ClientsPropertiesBySavedLinkIdGet
      x-api-path-slug: clientspropertiessavedlinkid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Properties
      - Saved
      - Link
  /partners/aggregatedproperties:
    get:
      summary: Get Partners Aggregated Properties
      description: Get a list of all lead saved properties.
      operationId: PartnersAggregatedpropertiesGet
      x-api-path-slug: partnersaggregatedproperties-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Properties
  /leads/property/{leadId}:
    get:
      summary: Get Leads Property
      description: Get a property information for a lead.
      operationId: LeadsPropertyByLeadIdGet
      x-api-path-slug: leadspropertyleadid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
    put:
      summary: Put Leads Property
      description: Add new property information for a lead.
      operationId: LeadsPropertyByLeadIdPut
      x-api-path-slug: leadspropertyleadid-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: formData
        name: propertyName
      - in: formData
        name: property[idxID]
      - in: formData
        name: property[listingID]
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
  /leads/property/{leadId}/{propId}:
    post:
      summary: Post Leads Property
      description: Update a property information for a lead.
      operationId: LeadsPropertyByLeadIdAndPropIdPost
      x-api-path-slug: leadspropertyleadidpropid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: formData
        name: propertyName
      - in: formData
        name: property[idxID]
      - in: formData
        name: property[listingID]
      - in: path
        name: propId
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
    delete:
      summary: Delete Leads Property
      description: Delete a property information for a lead.
      operationId: LeadsPropertyByLeadIdAndPropIdDelete
      x-api-path-slug: leadspropertyleadidpropid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: path
        name: propId
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
  /partners/propertytypes:
    get:
      summary: Get Partners Property Types
      description: Gives the names and IDs of all available property types. This method
        differs from the property type lookup method in the client API component in
        that it can look up property types for any active Platinum MLS, not just those
        for which the client is a member.
      operationId: PartnersPropertytypesGet
      x-api-path-slug: partnerspropertytypes-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Property
      - Types
  /mls/propertycount/{approvedMLS}:
    get:
      summary: Get Mls Propertycount Approvedmls
      description: Gives a total number of listings available for a given city, county,
        or zipcode
      operationId: MlsPropertycountByApprovedMLSGet
      x-api-path-slug: mlspropertycountapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: query
        name: countSpecifier
      - in: query
        name: countType
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Propertycount
      - Approvedmls
  /mls/propertytypes/{approvedMLS}:
    get:
      summary: Get Mls Propertytypes Approvedmls
      description: Gives the property type information for all types that are available
        on a given MLS.
      operationId: MlsPropertytypesByApprovedMLSGet
      x-api-path-slug: mlspropertytypesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Propertytypes
      - Approvedmls
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