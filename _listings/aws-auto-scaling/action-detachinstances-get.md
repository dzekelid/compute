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
  /?Action=DetachInstances&k=1:
    get:
      summary: ' Detach Instances '
      description: Removes one or more instances from the specified Auto Scaling group
      operationId: detachInstances
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If True, the Auto Scaling group decrements the desired capacity
          value by the number of instances detached
        type: string
      responses:
        200:
          description: OK
      tags:
      - server instances
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