---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global News Get Historical Market Headlines By Sector
  description: Returns all market headlines that were published in a specified time
    frame for a specified sector.
  version: 1.0.0
host: globalnews.xignite.com
basePath: xGlobalNews.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalReleasesBySecurity:
    get:
      summary: Get Historical Releases By Security
      description: Return press releases headlines for a security and a date range.
      operationId: GetHistoricalReleasesBySecurity
      x-api-path-slug: gethistoricalreleasesbysecurity-get
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
      - Releases
      - Security
  /GetHistoricalSecurityHeadlines:
    get:
      summary: Get Historical Security Headlines
      description: Returns all headlines that were published in a specified time frame
        for a given security.
      operationId: GetHistoricalSecurityHeadlines
      x-api-path-slug: gethistoricalsecurityheadlines-get
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
      - Security
      - Headlines
  /GetHistoricalMarketHeadlines:
    get:
      summary: Get Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: GetHistoricalMarketHeadlines
      x-api-path-slug: gethistoricalmarketheadlines-get
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
      - Market
      - Headlines
  /GetHistoricalMarketHeadlinesBySector:
    get:
      summary: Get Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: GetHistoricalMarketHeadlinesBySector
      x-api-path-slug: gethistoricalmarketheadlinesbysector-get
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
      - Market
      - Headlines
      - Sector
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