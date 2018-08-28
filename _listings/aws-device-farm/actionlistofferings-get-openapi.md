---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API List Offerings
  version: 1.0.0
  description: Returns a list of products or offerings that the user can manage through
    the API.
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