---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Put Groups
  description: Modifies a group. For example, you could change a group's title.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    delete:
      summary: Delete Groups
      description: Deletes a group.
      operationId: deleteGroups
      x-api-path-slug: groups-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube group ID for the group
          that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
    get:
      summary: Get Groups
      description: Returns a collection of groups that match the API request parameters.
        For example, you can retrieve all groups that the authenticated user owns,
        or you can retrieve one or more groups by their unique IDs.
      operationId: getGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          group ID(s) for the resource(s) that are being retrieved
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return groups owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Add Groups
      description: Creates a group.
      operationId: postGroups
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
    put:
      summary: Put Groups
      description: Modifies a group. For example, you could change a group's title.
      operationId: putGroups
      x-api-path-slug: groups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
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