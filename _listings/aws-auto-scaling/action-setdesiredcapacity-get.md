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
  /?Action=SetDesiredCapacity&k=1:
    get:
      summary: ' Set Desired Capacity '
      description: Sets the size of the specified Auto Scaling group
      operationId: setDesiredCapacity
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the Auto
          Scaling group
        type: string
      - in: query
        name: HonorCooldown
        description: By default, SetDesiredCapacity overrides any cooldown period
          associated with the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - desired capacity
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