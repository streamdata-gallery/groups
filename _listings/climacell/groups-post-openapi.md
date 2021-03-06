---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Post Groups
  description: |-
    ### Create a Group

    Creates a new Group, and name it. The system attaches a unique ID to each group you create. This ID is used to refer to the group and manage it in the following ```groups``` API calls.
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: Get Groups
      description: |-
        ### List all Groups
        Page through a list of all your groups. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-groupspage-through-a-list-of-all-your-groups-you-can-specify-the-maximum-number-of-results
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
    post:
      summary: Post Groups
      description: |-
        ### Create a Group

        Creates a new Group, and name it. The system attaches a unique ID to each group you create. This ID is used to refer to the group and manage it in the following ```groups``` API calls.
      operationId: -create-a-groupcreates-a-new-group-and-name-it-the-system-attaches-a-unique-id-to-each-group-you-cre
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
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