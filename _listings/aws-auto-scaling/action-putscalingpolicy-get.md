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
  /?Action=PutScalingPolicy&k=1:
    get:
      summary: ' Put Scaling Policy '
      description: Creates or updates a policy for an Auto Scaling group
      operationId: putScalingPolicy
      parameters:
      - in: query
        name: AdjustmentType
        description: The adjustment type
        type: string
      - in: query
        name: AutoScalingGroupName
        description: The name or ARN of the group
        type: string
      - in: query
        name: Cooldown
        description: The amount of time, in seconds, after a scaling activity completes
          and before the next scaling activity can start
        type: string
      - in: query
        name: EstimatedInstanceWarmup
        description: The estimated time, in seconds, until a newly launched instance
          can contribute to the CloudWatch metrics
        type: string
      - in: query
        name: MetricAggregationType
        description: The aggregation type for the CloudWatch metrics
        type: string
      - in: query
        name: MinAdjustmentMagnitude
        description: The minimum number of instances to scale
        type: string
      - in: query
        name: MinAdjustmentStep
        description: Available for backward compatibility
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy
        type: string
      - in: query
        name: PolicyType
        description: The policy type
        type: string
      - in: query
        name: ScalingAdjustment
        description: The amount by which to scale, based on the specified adjustment
          type
        type: string
      - in: query
        name: StepAdjustments.member.N
        description: A set of adjustments that enable you to scale based on the size
          of the alarm breach
        type: string
      responses:
        200:
          description: OK
      tags:
      - scaling policy
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