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
  /?Action=RebootInstances&k=1:
    get:
      summary: Reboot Instances
      description: Requests a reboot of one or more instances
      operationId: rebootinstances
      parameters:
      - in: query
        name: Description
        description: Descriptive text about the health state of your instance
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: EndTime
        description: The time at which the reported instance health state ended
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instances
        type: string
      - in: query
        name: ReasonCode.N
        description: One or more reason codes that describes the health state of your
          instance
        type: string
      - in: query
        name: StartTime
        description: The time at which the reported instance health state began
        type: string
      - in: query
        name: Status
        description: The status of all instances listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - instance
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