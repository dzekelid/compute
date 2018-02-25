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
  /?Action=SetRulePriorities&k=1:
    get:
      summary: ' Set Rule Priorities '
      description: Sets the priorities of the specified rules
      operationId: setRulePriorities
      parameters:
      - in: query
        name: RulePriorities.member.N
        description: The rule priorities
        type: string
      responses:
        200:
          description: OK
      tags:
      - rule priorities
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