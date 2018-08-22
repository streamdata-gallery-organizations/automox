---
swagger: "2.0"
x-collection-name: Automox
x-complete: 0
info:
  title: Automox Get Events
  description: Gets a specific `Event` object for the authenticated user.
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: Get Events
      description: Gets all `Event` objects for the authenticated user.
      operationId: gets-all-event-objects-for-the-authenticated-user
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Gets a specific `Event` object for the authenticated user.
      operationId: gets-a-specific-event-object-for-the-authenticated-user
      x-api-path-slug: eventsid-get
      parameters:
      - in: path
        name: id
        description: event ID
      responses:
        200:
          description: OK
      tags:
      - Events
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