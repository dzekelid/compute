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
  /?Action=RecordLifecycleActionHeartbeat&k=1:
    get:
      summary: ' Record Lifecycle Action Heartbeat '
      description: Records a heartbeat for the lifecycle action associated with the
        specified token or instance
      operationId: recordLifecycleActionHeartbeat
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group for the hook
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: LifecycleActionToken
        description: A token that uniquely identifies a specific lifecycle action
          associated with an instance
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - life cycle
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