swagger: "2.0"
x-collection-name: Intrinio
x-complete: 1
info:
  title: Intrinio
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /prices/exchange:
    get:
      summary: Exchange Prices
      description: Returns professional-grade historical stock prices for all securities
        traded on a stock exchange for a single specified day.  Historical prices
        are available back to 1996 or the IPO date, with some companies with data
        back to the 1970s.
      operationId: exchange-prices
      x-api-path-slug: pricesexchange-get
      parameters:
      - in: query
        name: identifier
        description: 'the stock market ticker symbol associated with the companies
          common stock securities or the stock market index:'
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: price_date
        description: the specified date in which historical stock prices are returned
          for a stock exchange
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Prices
      - Exchanges