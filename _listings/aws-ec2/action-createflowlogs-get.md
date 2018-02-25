---
swagger: "2.0"
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateFlowLogs&k=1:
    get:
      summary: Create Flow Logs
      description: Creates one or more flow logs to capture IP traffic for a specific
        network interface, subnet, or VPC
      operationId: createflowlogs
      parameters:
      - in: query
        name: FlowLogId.N
        description: One or more flow log IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - flow logs
definitions: []
x-collection-name: AWS EC2
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