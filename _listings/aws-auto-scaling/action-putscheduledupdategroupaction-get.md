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
  /?Action=PutScheduledUpdateGroupAction&k=1:
    get:
      summary: ' Put Scheduled Update Group Action '
      description: Creates or updates a scheduled scaling action for an Auto Scaling
        group
      operationId: putScheduledUpdateGroupAction
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the group
        type: string
      - in: query
        name: EndTime
        description: The time for the recurring schedule to end
        type: string
      - in: query
        name: MaxSize
        description: The maximum size for the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size for the Auto Scaling group
        type: string
      - in: query
        name: Recurrence
        description: The recurring schedule for this action, in Unix cron syntax format
        type: string
      - in: query
        name: ScheduledActionName
        description: The name of this scaling action
        type: string
      - in: query
        name: StartTime
        description: The time for this action to start, in YYYY-MM-DDThh:mm:ssZ format
          in UTC/GMT only             (for example, 2014-06-01T00:00:00Z)
        type: string
      - in: query
        name: Time
        description: This parameter is deprecated
        type: string
      responses:
        200:
          description: OK
      tags:
      - scheduled update
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