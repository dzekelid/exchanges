---
name: CoinMarketCap
x-slug: coinmarketcap
description: Cryptocurrency market cap rankings, charts, and more
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
x-kinRank: "7"
x-alexaRank: "276"
tags: Exchanges
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/exchanges/master/_listings/coinmarketcap/apis.md
specificationVersion: "0.14"
apis:
- name: CoinMarketCap Professional API Documentation - List all exchanges (latest)
  x-api-slug: v1exchangelistingslatest-get
  description: "Get a paginated list of all cryptocurrency exchanges with 24 hour
    volume. Additional market data fields will be available in the future. You can
    configure this call to sort by 24 hour volume or another field. Use the \"convert\"
    option to return market values in multiple fiat and cryptocurrency conversions
    in the same call.  \n  \n**This endpoint is available on the following API plans:**\n
    \ - ~~Starter~~\n  - ~~Hobbyist~~\n  - Standard\n  - Professional\n  - Enterprise\n\n**Cache
    / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute
    updates shortly.  \n  \n  *NOTE: Use this endpoint if you need a sorted and paginated
    list of exchanges. If you want to query for market data on a few specific exchanges
    use /v1/exchange/quotes/latest which is optimized for that purpose. The response
    data between these endpoints is otherwise the same.*"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/exchanges/master/_listings/coinmarketcap/v1exchangelistingslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/exchanges/master/_listings/coinmarketcap/v1exchangelistingslatest-get-openapi.md
- name: CoinMarketCap Professional API Documentation - List all exchanges (historical)
  x-api-slug: v1exchangelistingshistorical-get
  description: |-
    **This endpoint is not yet available. It is slated for release in Q3 2018.**


    Get a paginated list of all cryptocurrency exchanges with historical market data for a given point in time. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/exchanges/master/_listings/coinmarketcap/v1exchangelistingshistorical-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/exchanges/master/_listings/coinmarketcap/v1exchangelistingshistorical-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/coinmarketcap
- type: x-openapi
  url: https://pro-api.coinmarketcap.com/swagger.json
- type: x-api-gallery
  url: http://coinfabrik.api.gallery.streamdata.io
- type: x-email
  url: legal@coinmarketcap.com
- type: x-twitter
  url: https://twitter.com/CoinMarketCap
- type: x-website
  url: https://pro.coinmarketcap.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---