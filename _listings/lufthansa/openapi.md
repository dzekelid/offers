swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Public
  version: "1.0"
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /promotions/priceoffers/flights/ond/{origin}/{destination}:
    get:
      summary: Price Offers
      description: Retrieve a best price offer given an origin and destination.
      operationId: promotions.priceoffers.flights.ond.origin.destination.get
      x-api-path-slug: promotionspriceoffersflightsondorigindestination-get
      parameters:
      - in: query
        name: departureDate
        description: Departure date in local time (YYYY-MM-DD)
      - in: path
        name: destination
        description: Destination city
      - in: path
        name: origin
        description: Departure city
      - in: query
        name: returnDate
        description: Return date in local time (YYYY-MM-DD)
      - in: query
        name: service
        description: Optional parameter
      responses:
        200:
          description: OK
      tags:
      - Price
      - Offers
  /offers/lounges/{location}:
    get:
      summary: Lounges
      description: Lounge information
      operationId: OffersLoungesByLocationGet
      x-api-path-slug: offersloungeslocation-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabinClass
        description: 'Cabin class: M, E, C, F (Acceptable values are: , M, E, C, F)'
      - in: query
        name: lang
        description: Language code
      - in: path
        name: location
        description: 3-leter IATA airport or city code (e
      - in: query
        name: tierCode
        description: 'Frequent flyer level (FTL, SGC, SEN, HON) (Acceptable values
          are: , FTL, SGC, SEN, HON)'
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Lounges
      - Location
  /offers/seatmaps/{flightNumber}/{origin}/{destination}/{date}/{cabinClass}:
    get:
      summary: Seat Maps
      description: Cabin layout and seat characteristics.
      operationId: OffersSeatmapsDestinationDateCabinClassByFlightNumberAndOriginGet
      x-api-path-slug: offersseatmapsflightnumberorigindestinationdatecabinclass-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: cabinClass
        description: 'Cabin class: M, E, C, F'
      - in: path
        name: date
        description: Departure date (YYYY-MM-DD)
      - in: path
        name: destination
        description: Destination airport
      - in: path
        name: flightNumber
        description: Flight number including carrier code and any suffix (e
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Seatmaps
      - FlightNumber
      - Origin
      - Destination
      - Date
      - CabinClass