---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Get Package Offers
  description: Mobile API Packages
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/packages/hotelOffers:
    get:
      summary: Get Package Offers
      description: Mobile API Packages
      operationId: packages-offers
      x-api-path-slug: apipackageshoteloffers-get
      parameters:
      - in: query
        name: checkInDate
        description: Date the traveler will be checking in to their hotel
      - in: query
        name: checkOutDate
        description: Date the traveler will be checking out of their hotel
      - in: query
        name: childTravelerAge
        description: childTravelerAge represents the age of a single child traveler
      - in: query
        name: infantSeatingInLap
        description: Set to true if infant(s) are without a reserved seat (in an adults
          lap)
      - in: query
        name: numberOfAdultTravelers
        description: 'Number of Adult Travelers (Default: 1)'
      - in: query
        name: productKey
        description: The product ID (piid) of the package you would like to get hotel
          offers for
      - in: query
        name: ratePlanCode
        description: Rate Plan Code of the selected hotel offer
      - in: query
        name: roomTypeCode
        description: Room Type Code of the selected hotel offer
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Packages
      - Offers
      - Hotels
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