---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get historical prices for a property by its Id
  version: 1.0.0
  description: Get historical prices for a property by its id.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/{id}/historicalprices:
    get:
      summary: Get historical prices for a property by its Id
      description: Get historical prices for a property by its id.
      operationId: HistoricalPrice_GetByPropertyIdByidBypageNumberBypageSize
      x-api-path-slug: apipropertyidhistoricalprices-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Pricesa
      - Property
      - By
      - Its
      - Id
  /api/property/historicalprices/postcode/{postcode}:
    get:
      summary: Get historical prices for a property by its Id
      description: Get historical prices for a property by its id.
      operationId: HistoricalPrice_GetByPostcodeBypostcodeBypropertyTypeBystyleTypeByleaseTypeBypageNumberBypageSize
      x-api-path-slug: apipropertyhistoricalpricespostcodepostcode-get
      parameters:
      - in: query
        name: leaseType
        description: 'Options are: Freehold, Leasehold'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: path
        name: postcode
        description: The postcode to get historical price data for
      - in: query
        name: propertyType
        description: 'Options are: DetachedHouse, SemiDetachedHouse, TerracedHouse,
          Flat'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: styleType
        description: 'Options are: New, Older'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Pricesa
      - Property
      - By
      - Its
      - Id
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