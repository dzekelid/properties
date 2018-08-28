---
name: ATTOM
x-slug: attom
description: 'Search public property records including real estate data: sale, ownership,
  tax, and more - for more than 150 million U.S. properties. ATTOM Data Solutions
  is the curator of ATTOM, a multi-sourced national property data warehouse that contains
  tax, deed, mortgage, foreclosure, environmental risk, natural hazard, health hazard,
  neighborhood characteristic and property characteristic data for over 155 million
  U.S. properties, delivering actionable data to clients and powering consumer websites
  owned by ATTOM Data Solutions: RealtyTrac.com, Homefacts.com, and HomeDisclosure.com.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
x-kinRank: "7"
x-alexaRank: "359677"
tags: Properties
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/apis.md
specificationVersion: "0.14"
apis:
- name: Attom Data Solutions API - Returns a list of properties that fit a criteria.
  x-api-slug: propertyid-get
  description: Get a list of property IDs within a specific geography that have a
    specific number of beds. Use orderby to choose how you want your results sorted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyid-get-openapi.md
- name: Attom Data Solutions API - Returns properties within a zip code.
  x-api-slug: propertyaddress-get
  description: Get a list of properties within a zip code. Use propertytype and order
    by to narrow down your results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyaddress-get-openapi.md
- name: Attom Data Solutions API - Returns properties and their characteristics that
    fit a criteria.
  x-api-slug: propertysnapshot-get
  description: Get a list of property snapshots within a specific city that are within
    a desired size range and a specific property type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertysnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns property details based on an ID.
  x-api-slug: propertydetail-get
  description: Get property details based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetail-get-openapi.md
- name: Attom Data Solutions API - Returns basic property information and most recent
    transaction and taxes.
  x-api-slug: propertybasicprofile-get
  description: Get basic property information and most recent transaction and taxes
    for a specific attom id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertybasicprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertybasicprofile-get-openapi.md
- name: Attom Data Solutions API - Returns detailed property information and most
    recent transaction and taxes.
  x-api-slug: propertyexpandedprofile-get
  description: Get a detailed property information and most recent transaction and
    taxes for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyexpandedprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyexpandedprofile-get-openapi.md
- name: Attom Data Solutions API - Return schools within the attendance boundary of
    a property.
  x-api-slug: propertydetailwithschools-get
  description: Search for a property to have the property details returned, along
    with the schools in the associated attendance zones.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailwithschools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailwithschools-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgage based on ID.
  x-api-slug: propertydetailmortgage-get
  description: Get property details mortgage based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgage-get-openapi.md
- name: Attom Data Solutions API - Returns property details owner based on an ID.
  x-api-slug: propertydetailowner-get
  description: Get property details owner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailowner-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgageowner based on
    an ID.
  x-api-slug: propertydetailmortgageowner-get
  description: Get property details mortgageowner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgageowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgageowner-get-openapi.md
- name: Attom Data Solutions API - Returns assessment history and property details.
  x-api-slug: assessmenthistorydetail-get
  description: Get a full detail of property characteristics and assessment history
    information for a specific property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/assessmenthistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/assessmenthistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns AVM details for a property.
  x-api-slug: avmdetail-get
  description: Get AVM details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/avmdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/avmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns the Attomized AVM and other property details
    .
  x-api-slug: attomavmdetail-get
  description: Get Attomized AVM and other property details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/attomavmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns sale information for a property.
  x-api-slug: saledetail-get
  description: Get sales information for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saledetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saledetail-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorysnapshot-get
  description: Get a sales history snapshot of a property based on an Onboard property
    ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorysnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns basic transaction and loan history on a
    property.
  x-api-slug: saleshistorybasichistory-get
  description: Get the basic transaction and loan history on a property for a specific
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorybasichistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorybasichistory-get-openapi.md
- name: Attom Data Solutions API - Returns detailed transaction, pre-foreclosure and
    loan history on a property.
  x-api-slug: saleshistoryexpandedhistory-get
  description: Get the detailed transaction, pre-foreclosure and loan history on a
    property for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistoryexpandedhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistoryexpandedhistory-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorydetail-get
  description: Get a sales history snapshot of a property based on an address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns property details based on an ID.
  x-api-slug: propertydetail-get
  description: Get property details based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetail-get-openapi.md
- name: Attom Data Solutions API - Returns basic property information and most recent
    transaction and taxes.
  x-api-slug: propertybasicprofile-get
  description: Get basic property information and most recent transaction and taxes
    for a specific attom id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertybasicprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertybasicprofile-get-openapi.md
- name: Attom Data Solutions API - Returns detailed property information and most
    recent transaction and taxes.
  x-api-slug: propertyexpandedprofile-get
  description: Get a detailed property information and most recent transaction and
    taxes for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyexpandedprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyexpandedprofile-get-openapi.md
- name: Attom Data Solutions API - Return schools within the attendance boundary of
    a property.
  x-api-slug: propertydetailwithschools-get
  description: Search for a property to have the property details returned, along
    with the schools in the associated attendance zones.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailwithschools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailwithschools-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgage based on ID.
  x-api-slug: propertydetailmortgage-get
  description: Get property details mortgage based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgage-get-openapi.md
- name: Attom Data Solutions API - Returns property details owner based on an ID.
  x-api-slug: propertydetailowner-get
  description: Get property details owner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailowner-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgageowner based on
    an ID.
  x-api-slug: propertydetailmortgageowner-get
  description: Get property details mortgageowner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgageowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgageowner-get-openapi.md
- name: Attom Data Solutions API - Returns assessment history and property details.
  x-api-slug: assessmenthistorydetail-get
  description: Get a full detail of property characteristics and assessment history
    information for a specific property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/assessmenthistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/assessmenthistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns AVM details for a property.
  x-api-slug: avmdetail-get
  description: Get AVM details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/avmdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/avmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns the Attomized AVM and other property details
    .
  x-api-slug: attomavmdetail-get
  description: Get Attomized AVM and other property details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/attomavmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns sale information for a property.
  x-api-slug: saledetail-get
  description: Get sales information for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saledetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saledetail-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorysnapshot-get
  description: Get a sales history snapshot of a property based on an Onboard property
    ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorysnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns basic transaction and loan history on a
    property.
  x-api-slug: saleshistorybasichistory-get
  description: Get the basic transaction and loan history on a property for a specific
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorybasichistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorybasichistory-get-openapi.md
- name: Attom Data Solutions API - Returns detailed transaction, pre-foreclosure and
    loan history on a property.
  x-api-slug: saleshistoryexpandedhistory-get
  description: Get the detailed transaction, pre-foreclosure and loan history on a
    property for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistoryexpandedhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistoryexpandedhistory-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorydetail-get
  description: Get a sales history snapshot of a property based on an address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorydetail-get
  description: Get a sales history snapshot of a property based on an address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns detailed transaction, pre-foreclosure and
    loan history on a property.
  x-api-slug: saleshistoryexpandedhistory-get
  description: Get the detailed transaction, pre-foreclosure and loan history on a
    property for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistoryexpandedhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistoryexpandedhistory-get-openapi.md
- name: Attom Data Solutions API - Returns basic transaction and loan history on a
    property.
  x-api-slug: saleshistorybasichistory-get
  description: Get the basic transaction and loan history on a property for a specific
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorybasichistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorybasichistory-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorysnapshot-get
  description: Get a sales history snapshot of a property based on an Onboard property
    ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saleshistorysnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns sale information for a property.
  x-api-slug: saledetail-get
  description: Get sales information for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saledetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/saledetail-get-openapi.md
- name: Attom Data Solutions API - Returns the Attomized AVM and other property details
    .
  x-api-slug: attomavmdetail-get
  description: Get Attomized AVM and other property details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/attomavmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns AVM details for a property.
  x-api-slug: avmdetail-get
  description: Get AVM details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/avmdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/avmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns assessment history and property details.
  x-api-slug: assessmenthistorydetail-get
  description: Get a full detail of property characteristics and assessment history
    information for a specific property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/assessmenthistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/assessmenthistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgageowner based on
    an ID.
  x-api-slug: propertydetailmortgageowner-get
  description: Get property details mortgageowner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgageowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgageowner-get-openapi.md
- name: Attom Data Solutions API - Returns property details owner based on an ID.
  x-api-slug: propertydetailowner-get
  description: Get property details owner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailowner-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgage based on ID.
  x-api-slug: propertydetailmortgage-get
  description: Get property details mortgage based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailmortgage-get-openapi.md
- name: Attom Data Solutions API - Return schools within the attendance boundary of
    a property.
  x-api-slug: propertydetailwithschools-get
  description: Search for a property to have the property details returned, along
    with the schools in the associated attendance zones.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailwithschools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetailwithschools-get-openapi.md
- name: Attom Data Solutions API - Returns detailed property information and most
    recent transaction and taxes.
  x-api-slug: propertyexpandedprofile-get
  description: Get a detailed property information and most recent transaction and
    taxes for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyexpandedprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertyexpandedprofile-get-openapi.md
- name: Attom Data Solutions API - Returns basic property information and most recent
    transaction and taxes.
  x-api-slug: propertybasicprofile-get
  description: Get basic property information and most recent transaction and taxes
    for a specific attom id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertybasicprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertybasicprofile-get-openapi.md
- name: Attom Data Solutions API - Returns property details based on an ID.
  x-api-slug: propertydetail-get
  description: Get property details based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/properties/master/_listings/attom/propertydetail-get-openapi.md
x-common:
- type: x-openapi
  url: https://api.developer.attomdata.com/swagger/spec/propertyapi_property.json
- type: x-api-gallery
  url: http://atlassian.api.gallery.streamdata.io
- type: x-api-stack
  url: http://attom.stack.network
- type: x-email
  url: privacy@attomdata.com
- type: x-twitter
  url: https://twitter.com/Attomdata
- type: x-website
  url: https://api.developer.attomdata.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---