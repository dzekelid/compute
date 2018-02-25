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
  /?Action=DescribeAccountLimits&k=1:
    get:
      summary: ' Describe Account Limits '
      description: Describes the current Auto Scaling resource limits for your AWS
        account
      operationId: describeAccountLimits
      parameters:
      - in: query
        name: MaxNumberOfAutoScalingGroups
        description: The maximum number of groups allowed for your AWS account
        type: string
      - in: query
        name: MaxNumberOfLaunchConfigurations
        description: The maximum number of launch configurations allowed for your
          AWS account
        type: string
      - in: query
        name: NumberOfAutoScalingGroups
        description: The current number of groups for your AWS account
        type: string
      - in: query
        name: NumberOfLaunchConfigurations
        description: The current number of launch configurations for your AWS account
        type: string
      responses:
        200:
          description: OK
      tags:
      - account limits
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