---
swagger: "2.0"
x-collection-name: Automox
x-complete: 0
info:
  title: Automox Delete Servers
  description: ""
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
  /orgs:
    get:
      summary: Get Orgs
      description: Gets all organizations for the api key
      operationId: gets-all-organizations-for-the-api-key
      x-api-path-slug: orgs-get
      responses:
        200:
          description: OK
      tags:
      - Orgs
  /orgs/{id}/packages:
    get:
      summary: Get Orgs Packages
      description: Returns all software packages discovered on all servers (endpoints)
        of an organization
      operationId: returns-all-software-packages-discovered-on-all-servers-endpoints-of-an-organization
      x-api-path-slug: orgsidpackages-get
      parameters:
      - in: path
        name: id
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Packages
  /policies:
    get:
      summary: Get Policies
      description: Gets all `Policy` objects for authenticated user
      operationId: gets-all-policy-objects-for-authenticated-user
      x-api-path-slug: policies-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policies
  /policies/{id}:
    get:
      summary: Get Policies
      description: Gets a specific `Policy` object for the authenticated user.
      operationId: gets-a-specific-policy-object-for-the-authenticated-user
      x-api-path-slug: policiesid-get
      parameters:
      - in: path
        name: id
        description: Policy ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policies
    put:
      summary: Put Policies
      description: Updates a `Policy` object
      operationId: updates-a-policy-object
      x-api-path-slug: policiesid-put
      parameters:
      - in: path
        name: id
        description: Policy ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: policy
        description: Updated policy object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Policies
  /policies/{id}/action:
    post:
      summary: Post Policies Action
      description: Schedule a policy for immediate remediation
      operationId: schedule-a-policy-for-immediate-remediation
      x-api-path-slug: policiesidaction-post
      parameters:
      - in: formData
        name: action
        description: Remediation action type [remediateAll]
      - in: path
        name: id
        description: Policy ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policies
      - Action
  /policysets:
    get:
      summary: Get Policysets
      description: Gets all `Policy Set` objects for authenticated user
      operationId: gets-all-policy-set-objects-for-authenticated-user
      x-api-path-slug: policysets-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policysets
  /policystats:
    get:
      summary: Get Policystats
      description: Gets all `Policy Stats` objects for authenticated user
      operationId: gets-all-policy-stats-objects-for-authenticated-user
      x-api-path-slug: policystats-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policystats
  /servers:
    get:
      summary: Get Servers
      description: Gets all `Server` objects for authenticated user
      operationId: gets-all-server-objects-for-authenticated-user
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}:
    get:
      summary: Get Servers
      description: Gets a specific `Server` object for the authenticated user.
      operationId: gets-a-specific-server-object-for-the-authenticated-user
      x-api-path-slug: serversid-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
    put:
      summary: Put Servers
      description: Updates a `Server` object
      operationId: updates-a-server-object
      x-api-path-slug: serversid-put
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: server
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
    delete:
      summary: Delete Servers
      description: ""
      operationId: ""
      x-api-path-slug: serversid-delete
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
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