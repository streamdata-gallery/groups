---
swagger: "2.0"
info:
  title: Meetup Member groups
  description: |-
    Lists the authenticated member's groups in the order of leadership,
    next upcoming event, then alphabetical order by name
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /self/groups:
    get:
      summary: Member groups
      description: |-
        Lists the authenticated member's groups in the order of leadership,
        next upcoming event, then alphabetical order by name
      operationId: groups
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: page
        description: Number of groups to return in a single page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - members
      - groups
definitions: []
x-collection-name: Meetup
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