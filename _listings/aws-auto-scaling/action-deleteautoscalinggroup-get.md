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
  /?Action=DeleteAutoScalingGroup&k=1:
    get:
      summary: ' Delete Auto Scaling Group '
      description: Deletes the specified Auto Scaling group
      operationId: deleteAutoScalingGroup
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group to delete
        type: string
      - in: query
        name: ForceDelete
        description: Specifies that the group will be deleted along with all instances
          associated with the group, without waiting for all instances to be terminated
        type: string
      responses:
        200:
          description: OK
      tags:
      - auto scaling groups
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