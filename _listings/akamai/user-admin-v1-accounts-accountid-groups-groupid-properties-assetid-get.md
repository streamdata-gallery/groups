---
swagger: "2.0"
info:
  title: Akamai API Get a Property
  description: Get a Property
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user-admin/v1/accounts/{accountId}/groups/{groupId}/properties/{assetId}:
    get:
      summary: Get a Property
      description: Get a Property
      operationId: useradminv1accountsaccountidgroupsgroupidpropertiesassetid
      parameters:
      - in: query
        name: accountId
        description: Unique identifier for an account
        type: string
      - in: query
        name: assetId
        description: Within the User Admin API, the assetId is also known as the propertyId
        type: string
      - in: query
        name: groupId
        description: Unique numeric identifier for a group
        type: string
      responses:
        200:
          description: OK
      tags:
      - user
      - admin
      - accounts
      - account
      - groups
      - group
      - properties
      - asset
definitions: []
x-collection-name: Akamai
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