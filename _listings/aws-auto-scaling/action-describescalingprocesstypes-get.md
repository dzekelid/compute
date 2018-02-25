---
swagger: "2.0"
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeScalingProcessTypes&k=1:
    get:
      summary: ' Describe Scaling Process Types '
      description: Describes the scaling process types for use with
      operationId: describeScalingProcessTypes
      parameters:
      - in: query
        name: Processes.member.N
        description: The names of the process types
        type: string
      responses:
        200:
          description: OK
      tags:
      - scaling process
definitions: []
x-collection-name: AWS Auto Scaling
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