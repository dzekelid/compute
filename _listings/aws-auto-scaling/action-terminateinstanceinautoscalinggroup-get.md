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
  /?Action=TerminateInstanceInAutoScalingGroup&k=1:
    get:
      summary: ' Terminate Instance In Auto Scaling Group '
      description: Terminates the specified instance and optionally adjusts the desired
        group size
      operationId: terminateInstanceInAutoScalingGroup
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If true, terminating the instance also decrements the size of
          the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - instance auto scaling
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