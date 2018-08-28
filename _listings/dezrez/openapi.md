swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/sales/exchange:
    post:
      summary: Exchanges a sales role
      description: Exchanges a sales role.
      operationId: SalesProgression_ExchangeByexchangeCommandDataContract
      x-api-path-slug: apiprogressionsalesexchange-post
      parameters:
      - in: body
        name: exchangeCommandDataContract
        description: Details of the exchange
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Exchanges
      - Sales
      - Role