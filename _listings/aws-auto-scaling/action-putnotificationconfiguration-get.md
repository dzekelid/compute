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
  /?Action=PutNotificationConfiguration&k=1:
    get:
      summary: ' Put Notification Configuration '
      description: Configures an Auto Scaling group to send notifications when specified
        events take place
      operationId: putNotificationConfiguration
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: NotificationTypes.member.N
        description: The type of event that will cause the notification to be sent
        type: string
      - in: query
        name: TopicARN
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - notifications
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