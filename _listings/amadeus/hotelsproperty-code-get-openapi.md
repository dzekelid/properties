---
swagger: "2.0"
x-collection-name: Amadeus
x-complete: 0
info:
  title: Amadeus Get Hotels Property Code
  description: "This API allows you to quickly see the detailed information of a single
    hotel, including descriptions, address, GPS location, amenities, awards, lowest
    priced room and all room prices and booking information. \n\nThis API gives you
    more information on a specific property. Optional parameters such as show_sold_out
    & rooms can be used to show sold out rooms and all available rooms. \n\nThe API
    is based on our high-speed hotel pricing cache, which is also used to power the
    Amadeus Hotel Search Engine application. Results are returned very quickly, response
    times are generally under 2s. Our cache has great global coverage and is constantly
    refreshed with the latest prices."
  contact:
    name: Amadeus Innovation and Research
    url: https://sandbox.amadeus.com
  version: 1.0.0
host: api.sandbox.amadeus.com
basePath: /v1.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hotels/{property_code}:
    get:
      summary: Get Hotels Property Code
      description: "This API allows you to quickly see the detailed information of
        a single hotel, including descriptions, address, GPS location, amenities,
        awards, lowest priced room and all room prices and booking information. \n\nThis
        API gives you more information on a specific property. Optional parameters
        such as show_sold_out & rooms can be used to show sold out rooms and all available
        rooms. \n\nThe API is based on our high-speed hotel pricing cache, which is
        also used to power the Amadeus Hotel Search Engine application. Results are
        returned very quickly, response times are generally under 2s. Our cache has
        great global coverage and is constantly refreshed with the latest prices."
      operationId: getHotelsPropertyCode
      x-api-path-slug: hotelsproperty-code-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: path
        name: property_code
        description: A Hotel property code based on 2 letter chain code + 3 letter
          IATA code of the city + 3 char property unique id
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Property
      - Code
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