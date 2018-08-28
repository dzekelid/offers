swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeHostReservationOfferings:
    get:
      summary: Describe Host Reservation Offerings
      description: Describes the Dedicated Host Reservations that are available to
        purchase.
      operationId: describehostreservationofferings
      x-api-path-slug: actiondescribehostreservationofferings-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: HostReservationIdSet.N
        description: One or more host reservation IDs
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Host Reservation
  /?Action=DescribeReservedInstancesOfferings:
    get:
      summary: Describe Reserved Instances Offerings
      description: Describes Reserved Instance offerings that are available for purchase.
      operationId: describereservedinstancesofferings
      x-api-path-slug: actiondescribereservedinstancesofferings-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: ReservedInstanceId.N
        description: The IDs of the Convertible Reserved Instances to exchange
        type: string
      - in: query
        name: TargetConfiguration.N
        description: The configuration requirements of the Convertible Reserved Instances
          to exchange for your current      Convertible Reserved Instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=PurchaseReservedInstancesOffering:
    get:
      summary: Purchase Reserved Instances Offering
      description: Purchases a Reserved Instance for use with your account.
      operationId: purchasereservedinstancesoffering
      x-api-path-slug: actionpurchasereservedinstancesoffering-get
      parameters:
      - in: query
        name: PrincipalArn
        description: The ARN of the principal, which can be an IAM role, IAM user,
          or the root user
        type: string
      - in: query
        name: Resource
        description: 'The type of resource: instance | reservation |        snapshot
          | volume'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance