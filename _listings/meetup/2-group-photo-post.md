---
swagger: "2.0"
info:
  title: Meetup Group Photo Upload
  description: Uploads a new Meetup Group photo. To change other Group settings use
    the [Group Edit](/meetup_api/docs/:urlname/#edit) endpoint
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
  /2/group_photo:
    post:
      summary: Group Photo Upload
      description: Uploads a new Meetup Group photo
      operationId: groups
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: group_id
        description: Group ID for the target group
        type: string
      - in: query
        name: group_urlname
        description: Group urlname
        type: string
      - in: query
        name: main
        description: Set to 'true' to have this photo become the group's main photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
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