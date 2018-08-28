swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/offers:
    get:
      summary: Get Account Offers
      description: Get Offers related to an account
      operationId: GetAccountOffers
      x-api-path-slug: accountsaccountidoffers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Offers
  /offers:
    get:
      summary: Get Offers
      description: Get Offers
      operationId: GetOffers
      x-api-path-slug: offers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Offers