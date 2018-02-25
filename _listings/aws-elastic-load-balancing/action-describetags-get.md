---
swagger: "2.0"
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTags&k=1:
    get:
      summary: ' Describe Tags '
      description: Describes the tags for the specified resources
      operationId: describeTags
      parameters:
      - in: query
        name: ResourceArns.member.N
        description: The Amazon Resource Names (ARN) of the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - tags
definitions: []
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