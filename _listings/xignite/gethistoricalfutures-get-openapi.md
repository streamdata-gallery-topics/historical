---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Historical Futures
  description: Returns historical quotes for multiple future contracts.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalFutureStrip:
    get:
      summary: Get Historical Future Strip
      description: Returns a future strip for a commodity.
      operationId: postGethistoricalfuturestrip
      x-api-path-slug: gethistoricalfuturestrip-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Strip
  /GetHistoricalSwapStrip:
    get:
      summary: Get Historical Swap Strip
      description: Returns a future strip for a commodity.
      operationId: postGethistoricalswapstrip
      x-api-path-slug: gethistoricalswapstrip-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Strip
  /GetHistoricalFuture:
    get:
      summary: Get Historical Future
      description: Returns a historical quote for a future contract.
      operationId: postGethistoricalfuture
      x-api-path-slug: gethistoricalfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
  /GetHistoricalFutures:
    get:
      summary: Get Historical Futures
      description: Returns historical quotes for multiple future contracts.
      operationId: postGethistoricalfutures
      x-api-path-slug: gethistoricalfutures-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Futures
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