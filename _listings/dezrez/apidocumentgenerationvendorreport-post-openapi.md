---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a correspondence to a single group, sending them a single
    report for multiple properties
  version: 1.0.0
  description: Generates a correspondence to a single group, sending them a single
    report for multiple properties.
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