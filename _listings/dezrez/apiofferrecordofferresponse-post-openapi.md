---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Record a sale/auction offer response
  version: 1.0.0
  description: Record a sale/auction offer response.
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
        200:
          description: OK
      tags:
      - Offers
      - By
      - Id
      - If
      - It
      - Exists
    get:
      summary: Get an offer by its id.
      description: Get an offer by its id..
      operationId: Offer_GetByid
      x-api-path-slug: apiofferid-get
      parameters:
      - in: path
        name: id
        description: The id of the Offer to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Offer
      - By
      - Its
      - Id
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
  /api/documentgeneration/offer:
    post:
      summary: Generates a correspondence notifying the vendor of an offer.  Uses
        default values where possible.
      description: Generates a correspondence notifying the vendor of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationoffer-post
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
      - Notifying
      - Vendor
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offeraccepted:
    post:
      summary: Generates a correspondence any parties of the acceptance of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the acceptance of an
        offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferAcceptedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferaccepted-post
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
      - Any
      - Parties
      - Of
      - Acceptance
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerrejected:
    post:
      summary: Generates a correspondence any parties of the rejection of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the rejection of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferRejectedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferrejected-post
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
      - Any
      - Parties
      - Of
      - Rejection
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerwithdrawn:
    post:
      summary: Generates a correspondence to notify any parties of the withdrawl of
        an offer.  Uses default values where possible.
      description: Generates a correspondence to notify any parties of the withdrawl
        of an offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferwithdrawnLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferwithdrawn-post
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
      - Notify
      - Any
      - Parties
      - Of
      - Withdrawl
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/offer/recordoffer:
    post:
      summary: Record offer on a sale
      description: Record offer on a sale.
      operationId: Offer_RecordOfferByofferCommand
      x-api-path-slug: apiofferrecordoffer-post
      parameters:
      - in: body
        name: offerCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Offer
      - "On"
      - Sale
  /api/offer/progressnoteofinterest:
    post:
      summary: Record a note against on a offer
      description: Record a note against on a offer.
      operationId: Offer_ProgressNoteOfInterestByofferIdBydataContract
      x-api-path-slug: apiofferprogressnoteofinterest-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: offerId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Note
      - Against
      - "On"
      - Offer
  /api/offer/reviseoffer:
    post:
      summary: Revise offer price
      description: Revise offer price.
      operationId: Offer_ReviseOfferByreviseOfferCommand
      x-api-path-slug: apiofferreviseoffer-post
      parameters:
      - in: body
        name: reviseOfferCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Revise
      - Offer
      - Price
  /api/offer/recordlettingoffer:
    post:
      summary: Record offer on a letting
      description: Record offer on a letting.
      operationId: Offer_RecordLettingOfferByofferCommand
      x-api-path-slug: apiofferrecordlettingoffer-post
      parameters:
      - in: body
        name: offerCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Offer
      - "On"
      - Letting
  /api/offer/recordofferresponse:
    post:
      summary: Record a sale/auction offer response
      description: Record a sale/auction offer response.
      operationId: Offer_RecordOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Sale
      - Auction
      - Offer
      - Response
  /api/offer/recordlettingofferresponse:
    post:
      summary: Record a letting offer response
      description: Record a letting offer response.
      operationId: Offer_RecordLettingOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordlettingofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Letting
      - Offer
      - Response
  /api/offer/recordauctionofferresponse:
    post:
      summary: Record a auction offer Response
      description: Record a auction offer response.
      operationId: Offer_RecordAuctionOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordauctionofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Auction
      - Offer
      - Response
  /api/Offer:
    get:
      summary: Gets a paged amount of offerss.
      description: Gets a paged amount of offerss..
      operationId: Offer_GetBypageSizeBypageNumber
      x-api-path-slug: apioffer-get
      parameters:
      - in: query
        name: pageNumber
        description: The page of offerss to return
      - in: query
        name: pageSize
        description: The number of offerss to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Paged
      - Amount
      - Of
      - Offerss
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