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
  /?Action=ExecutePolicy&k=1:
    get:
      summary: ' Execute Policy '
      description: Executes the specified policy
      operationId: executePolicy
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: BreachThreshold
        description: The breach threshold for the alarm
        type: string
      - in: query
        name: HonorCooldown
        description: If this parameter is true, Auto Scaling waits for the cooldown
          period to complete before executing the policy
        type: string
      - in: query
        name: MetricValue
        description: The metric value to compare to BreachThreshold
        type: string
      - in: query
        name: PolicyName
        description: The name or ARN of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - policies
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