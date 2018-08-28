---
name: Actility
x-slug: actility
description: 'Actility is the leader in low power wide area (LoRaWAN and 3GPP) network
  connectivity management for the Internet of Things: the ThingPark platform'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
x-kinRank: "7"
x-alexaRank: "637591"
tags: Offers
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/apis.md
specificationVersion: "0.14"
apis:
- name: ThingPark DX Core API - Offers retrieval
  x-api-slug: offers-get
  description: Retrieves a list of offers existing within authorized scopes. In case
    of a vendor scope, it retrieves all offers of that vendor. In case of a subscriber
    scope, it retrieves all offers subscribed by that subscriber.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offers-get-openapi.md
- name: ThingPark DX Core API - Offers creation
  x-api-slug: offers-post
  description: Creates a new offer. if not specified, 'state' is automatically set
    to 'ACTIVE'. Note that the offer id MUST start with the vendor id followed by
    a slash (e.g. 'vendor-id/offer-id').
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offers-post-openapi.md
- name: ThingPark DX Core API - Offer retrieval
  x-api-slug: offersofferref-get
  description: Retrieves the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-get-openapi.md
- name: ThingPark DX Core API - Offer update
  x-api-slug: offersofferref-put
  description: Updates the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes. Only 'name' and 'state' attributes can be updated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-put-openapi.md
- name: ThingPark DX Core API - Offer deletion
  x-api-slug: offersofferref-delete
  description: Deletes the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-delete-openapi.md
- name: ThingPark DX Core API - Offer retrieval
  x-api-slug: offersofferref-get
  description: Retrieves the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-get-openapi.md
- name: ThingPark DX Core API - Offer update
  x-api-slug: offersofferref-put
  description: Updates the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes. Only 'name' and 'state' attributes can be updated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-put-openapi.md
- name: ThingPark DX Core API - Offer deletion
  x-api-slug: offersofferref-delete
  description: Deletes the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-delete-openapi.md
- name: ThingPark DX Core API - Offer deletion
  x-api-slug: offersofferref-delete
  description: Deletes the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-delete-openapi.md
- name: ThingPark DX Core API - Offer update
  x-api-slug: offersofferref-put
  description: Updates the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes. Only 'name' and 'state' attributes can be updated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-put-openapi.md
- name: ThingPark DX Core API - Offer retrieval
  x-api-slug: offersofferref-get
  description: Retrieves the offer corresponding to the provided offer ref, if that
    offer is within authorized scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/offers/master/_listings/actility/offersofferref-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.actility.com/blog/feed/
- type: x-github
  url: https://github.com/actility
- type: x-openapi
  url: https://dx-api.thingpark.com/core/latest/tpdx-core-api-contract.json
- type: x-api-gallery
  url: http://actility.api.gallery.streamdata.io
- type: x-api-stack
  url: http://actility.stack.network
- type: x-blog
  url: https://www.actility.com/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/actility
- type: x-developer
  url: https://www.actility.com/developer/
- type: x-twitter
  url: https://twitter.com/Actility
- type: x-website
  url: https://www.actility.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---