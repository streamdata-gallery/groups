---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API Remove User From Group
  version: 1.0.0
  description: Removes the specified user from the specified group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveUserFromGroup:
    get:
      summary: ' Remove User From Group '
      description: Removes the specified user from the specified group
      operationId: removeUserFromGroup
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to update
        type: string
      - in: query
        name: UserName
        description: The name of the user to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - user from groups
definitions: []
x-collection-name: AWS Identity and Access Management
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