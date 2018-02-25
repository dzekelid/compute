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
  /?Action=PutLifecycleHook&k=1:
    get:
      summary: ' Put Lifecycle Hook '
      description: Creates or updates a lifecycle hook for the specified Auto Scaling
        Group
      operationId: putLifecycleHook
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group to which you want to assign
          the lifecycle hook
        type: string
      - in: query
        name: DefaultResult
        description: Defines the action the Auto Scaling group should take when the
          lifecycle hook timeout elapses or if an unexpected failure occurs
        type: string
      - in: query
        name: HeartbeatTimeout
        description: The amount of time, in seconds, that can elapse before the lifecycle
          hook times out
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      - in: query
        name: LifecycleTransition
        description: The instance state to which you want to attach the lifecycle
          hook
        type: string
      - in: query
        name: NotificationMetadata
        description: Contains additional information that you want to include any
          time Auto Scaling sends a message to the notification target
        type: string
      - in: query
        name: NotificationTargetARN
        description: The ARN of the notification target that Auto Scaling will use
          to notify you when an instance is in the transition state for the lifecycle
          hook
        type: string
      - in: query
        name: RoleARN
        description: The ARN of the IAM role that allows the Auto Scaling group to
          publish to the specified notification target
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