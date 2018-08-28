---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Offer deletion
  description: Deletes the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /offers:
    get:
      summary: Offers retrieval
      description: Retrieves a list of offers existing within authorized scopes. In
        case of a vendor scope, it retrieves all offers of that vendor. In case of
        a subscriber scope, it retrieves all offers subscribed by that subscriber.
      operationId: retrieves-a-list-of-offers-existing-within-authorized-scopes-in-case-of-a-vendor-scope-it-retrieves-
      x-api-path-slug: offers-get
      parameters:
      - in: query
        name: offerId
        description: Id of the offer to search for
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Retrieval
    post:
      summary: Offers creation
      description: Creates a new offer. if not specified, 'state' is automatically
        set to 'ACTIVE'. Note that the offer id MUST start with the vendor id followed
        by a slash (e.g. 'vendor-id/offer-id').
      operationId: creates-a-new-offer-if-not-specified-state-is-automatically-set-to-active-note-that-the-offer-id-mus
      x-api-path-slug: offers-post
      parameters:
      - in: body
        name: offer
        description: Contents of the offer to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Creation
  /offers/{offerRef}:
    get:
      summary: Offer retrieval
      description: Retrieves the offer corresponding to the provided offer ref, if
        that offer is within authorized scopes.
      operationId: retrieves-the-offer-corresponding-to-the-provided-offer-ref-if-that-offer-is-within-authorized-scope
      x-api-path-slug: offersofferref-get
      parameters:
      - in: path
        name: offerRef
        description: Ref of the offer to retrieve
      responses:
        200:
          description: OK
      tags:
      - Offer
      - Retrieval
    put:
      summary: Offer update
      description: Updates the offer corresponding to the provided offer ref, if that
        offer is within authorized scopes. Only 'name' and 'state' attributes can
        be updated.
      operationId: updates-the-offer-corresponding-to-the-provided-offer-ref-if-that-offer-is-within-authorized-scopes-
      x-api-path-slug: offersofferref-put
      parameters:
      - in: body
        name: offer
        description: Contents of the offer to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: offerRef
        description: Ref of the offer to update
      responses:
        200:
          description: OK
      tags:
      - Offer
      - Update
    delete:
      summary: Offer deletion
      description: Deletes the offer corresponding to the provided offer ref, if that
        offer is within authorized scopes.
      operationId: deletes-the-offer-corresponding-to-the-provided-offer-ref-if-that-offer-is-within-authorized-scopes
      x-api-path-slug: offersofferref-delete
      parameters:
      - in: path
        name: offerRef
        description: Ref of the offer to delete
      responses:
        200:
          description: OK
      tags:
      - Offer
      - Deletion
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