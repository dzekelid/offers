---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get a basic list of offers associated to the current property marketing
    role.
  version: 1.0.0
  description: Get a basic list of offers associated to the current property marketing
    role..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Offer/{id}:
    delete:
      summary: Delete an offers by id if it exists.
      description: Delete an offers by id if it exists..
      operationId: Offer_DeleteByid
      x-api-path-slug: apiofferid-delete
      parameters:
      - in: path
        name: id
        description: the offers id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Offers
      - By
      - Id
      - If
      - It
      - Exists
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