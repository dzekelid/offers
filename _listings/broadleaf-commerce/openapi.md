swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/{cartId}/offers:
    delete:
      summary: Delete Cart Offers
      description: Delete cart offers.
      operationId: deleteCartCartOffers
      x-api-path-slug: cartcartidoffers-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offers
  /cart/{cartId}/offer/{promoCode}:
    post:
      summary: Post Cart Offer Promocode
      description: Post cart offer promocode.
      operationId: postCartCartOfferPromocode
      x-api-path-slug: cartcartidofferpromocode-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: path
        name: promoCode
        description: promoCode
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offer
      - Promocode
    delete:
      summary: Delete Cart Offer Promocode
      description: Delete cart offer promocode.
      operationId: deleteCartCartOfferPromocode
      x-api-path-slug: cartcartidofferpromocode-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: path
        name: promoCode
        description: promoCode
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offer
      - Promocode