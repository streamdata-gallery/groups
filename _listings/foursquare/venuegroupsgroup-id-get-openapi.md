---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Venuegroups Group
  description: /venues/{VENUE_ID}/proposeedit
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /venuegroups/{GROUP_ID}:
    get:
      summary: Get Venuegroups Group
      description: /venues/{VENUE_ID}/proposeedit
      operationId: venuesvenue-idproposeedit
      x-api-path-slug: venuegroupsgroup-id-get
      parameters:
      - in: query
        name: GROUP_ID
        description: The ID of the venue group to retrieve additional information
          for
      - in: path
        name: GROUP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venuegroups
      - Group
  /venuegroups/{GROUP_ID}/addvenue:
    post:
      summary: Post Venuegroups Group Addvenue
      description: /venuegroups/list
      operationId: venuegroupslist
      x-api-path-slug: venuegroupsgroup-idaddvenue-post
      parameters:
      - in: query
        name: GROUP_ID
        description: The ID of the venue group
      - in: path
        name: GROUP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: Comma-delimited list of venue IDs to add to the group
      responses:
        200:
          description: OK
      tags:
      - Venuegroups
      - Group
      - Venue
  /venuegroups/{GROUP_ID}/delete:
    post:
      summary: Post Venuegroups Group Delete
      description: /venuegroups/add
      operationId: venuegroupsadd
      x-api-path-slug: venuegroupsgroup-iddelete-post
      parameters:
      - in: query
        name: GROUP_ID
        description: The ID of the venue group to delete
      - in: path
        name: GROUP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venuegroups
      - Group
  /venuegroups/{GROUP_ID}/removevenue:
    post:
      summary: Post Venuegroups Group Removevenue
      description: /venuegroups/{GROUP_ID}/addvenue
      operationId: venuegroupsgroup-idaddvenue
      x-api-path-slug: venuegroupsgroup-idremovevenue-post
      parameters:
      - in: query
        name: GROUP_ID
        description: The ID of the venue group
      - in: path
        name: GROUP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: Comma-delimited list of venue IDs to remove from the group
      responses:
        200:
          description: OK
      tags:
      - Venuegroups
      - Group
      - Removevenue
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