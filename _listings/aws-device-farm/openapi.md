swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetOfferingStatus:
    get:
      summary: Get Offering Status
      description: Gets the current status and future status of all offerings purchased
        by an AWS account.
      operationId: getOfferingStatus
      x-api-path-slug: actiongetofferingstatus-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offering Status
  /?Action=ListOfferings:
    get:
      summary: List Offerings
      description: Returns a list of products or offerings that the user can manage
        through the API.
      operationId: listOfferings
      x-api-path-slug: actionlistofferings-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings
  /?Action=ListOfferingTransactions:
    get:
      summary: List Offering Transactions
      description: |-
        Returns a list of all historical purchases, renewals, and system renewal transactions for an
              AWS account.
      operationId: listOfferingTransactions
      x-api-path-slug: actionlistofferingtransactions-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offering Transactions
  /?Action=PurchaseOffering:
    get:
      summary: Purchase Offering
      description: Immediately purchases offerings for an AWS account.
      operationId: purchaseOffering
      x-api-path-slug: actionpurchaseoffering-get
      parameters:
      - in: query
        name: offeringId
        description: The ID of the offering
        type: string
      - in: query
        name: quantity
        description: The number of device slots you wish to purchase in an offering
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings
  /?Action=RenewOffering:
    get:
      summary: Renew Offering
      description: |-
        Explicitly sets the quantity of devices to renew for an offering, starting from the
              effectiveDate of the next period.
      operationId: renewOffering
      x-api-path-slug: actionrenewoffering-get
      parameters:
      - in: query
        name: offeringId
        description: The ID of a request to renew an offering
        type: string
      - in: query
        name: quantity
        description: The quantity requested in an offering renewal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings