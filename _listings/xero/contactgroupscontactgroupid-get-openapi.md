---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Contact Groups
  description: Get contactgroups contactgroup.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ContactGroups:
    get:
      summary: Get Contactgroups
      description: Get contactgroups.
      operationId: getContactgroups
      x-api-path-slug: contactgroups-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
    post:
      summary: Post Contactgroups
      description: Post contactgroups.
      operationId: postContactgroups
      x-api-path-slug: contactgroups-post
      parameters:
      - in: body
        name: ContactGroups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
    put:
      summary: Put Contactgroups
      description: Put contactgroups.
      operationId: putContactgroups
      x-api-path-slug: contactgroups-put
      parameters:
      - in: body
        name: ContactGroups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
    x-related-model:
      summary: X-related-model Contactgroups
      description: X-related-model contactgroups.
      operationId: x-related-modelContactgroups
      x-api-path-slug: contactgroups-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
  /ContactGroups/{ContactGroupID}:
    delete:
      summary: Delete Contact Groups
      description: Delete contactgroups contactgroup.
      operationId: deleteContactgroupsContactgroup
      x-api-path-slug: contactgroupscontactgroupid-delete
      parameters:
      - in: path
        name: ContactGroupID
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
    get:
      summary: Get Contact Groups
      description: Get contactgroups contactgroup.
      operationId: getContactgroupsContactgroup
      x-api-path-slug: contactgroupscontactgroupid-get
      parameters:
      - in: path
        name: ContactGroupID
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
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