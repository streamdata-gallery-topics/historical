---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Meeting Get historical meetings by organizer
  description: 'Get historical meetings for the specified organizer that started within
    the specified date/time range. Remark: Meetings which are still ongoing at the
    time of the request are NOT contained in the result array.'
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2M/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{groupKey}/historicalMeetings:
    get:
      summary: Get historical meetings by group
      description: 'Get historical meetings for the specified group that started within
        the specified date/time range. This API call is only available to users with
        the admin role. This API call is restricted to groups with a maximum of 50
        organizers. Remark: Meetings which are still ongoing at the time of the request
        are NOT contained in the result array.'
      operationId: get-historical-meetings-for-the-specified-group-that-started-within-the-specified-datetime-range--th
      x-api-path-slug: groupsgroupkeyhistoricalmeetings-get
      parameters:
      - in: query
        name: endDate
        description: Required end of date range, in ISO8601 UTC format, e
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: Required start of date range, in ISO8601 UTC format, e
      responses:
        200:
          description: OK
      tags:
      - Groups
      - GroupKey
      - HistoricalMeetings
  /historicalMeetings:
    get:
      summary: Get historical meetings
      description: 'Get historical meetings for the currently authenticated organizer
        that started within the specified date/time range. Remark: Meetings which
        are still ongoing at the time of the request are NOT contained in the result
        array.'
      operationId: get-historical-meetings-for-the-currently-authenticated-organizer-that-started-within-the-specified-
      x-api-path-slug: historicalmeetings-get
      parameters:
      - in: query
        name: endDate
        description: Required end of date range, in ISO8601 UTC format, e
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: Required start of date range, in ISO8601 UTC format, e
      responses:
        200:
          description: OK
      tags:
      - HistoricalMeetings
  /organizers/{organizerKey}/historicalMeetings:
    get:
      summary: Get historical meetings by organizer
      description: 'Get historical meetings for the specified organizer that started
        within the specified date/time range. Remark: Meetings which are still ongoing
        at the time of the request are NOT contained in the result array.'
      operationId: get-historical-meetings-for-the-specified-organizer-that-started-within-the-specified-datetime-range
      x-api-path-slug: organizersorganizerkeyhistoricalmeetings-get
      parameters:
      - in: query
        name: endDate
        description: Required end of date range, in ISO8601 UTC format, e
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: Required start of date range, in ISO8601 UTC format, e
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - HistoricalMeetings
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