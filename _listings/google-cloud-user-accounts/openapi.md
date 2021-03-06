swagger: "2.0"
x-collection-name: Google Cloud User Accounts
x-complete: 1
info:
  title: Cloud User Accounts
  description: creates-and-manages-users-and-groups-for-accessing-google-compute-engine-virtual-machines-
  contact:
    name: Google
    url: https://google.com
  version: vm_alpha
host: www.googleapis.com
basePath: /clouduseraccounts/vm_alpha/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/groups:
    get:
      summary: Get Groups
      description: Retrieves the list of groups contained within the specified project.
      operationId: clouduseraccounts.groups.list
      x-api-path-slug: projectglobalgroups-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
    post:
      summary: Create Group
      description: Creates a Group resource in the specified project using the data
        included in the request.
      operationId: clouduseraccounts.groups.insert
      x-api-path-slug: projectglobalgroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
  /{project}/global/groups/{groupName}:
    delete:
      summary: Delete Group
      description: Deletes the specified Group resource.
      operationId: clouduseraccounts.groups.delete
      x-api-path-slug: projectglobalgroupsgroupname-delete
      parameters:
      - in: path
        name: groupName
        description: Name of the Group resource to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
    get:
      summary: Get Group
      description: Returns the specified Group resource.
      operationId: clouduseraccounts.groups.get
      x-api-path-slug: projectglobalgroupsgroupname-get
      parameters:
      - in: path
        name: groupName
        description: Name of the Group resource to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group