---
swagger: "2.0"
info:
  title: AWS Elastic Load Balancing API Describe Target Group Attributes
  version: 1.0.0
  description: Describes the attributes for the specified target group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTargetGroupAttributes:
    get:
      summary: ' Describe Target Group Attributes '
      description: Describes the attributes for the specified target group
      operationId: describeTargetGroupAttributes
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - target groups
definitions: []
x-collection-name: AWS Elastic Load Balancing
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