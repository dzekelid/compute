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
  /?Action=DescribeScheduledActions&k=1:
    get:
      summary: ' Describe Scheduled Actions '
      description: Describes the actions scheduled for your Auto Scaling group that
        haven't run
      operationId: describeScheduledActions
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: EndTime
        description: The latest scheduled start time to return
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ScheduledActionNames.member.N
        description: Describes one or more scheduled actions
        type: string
      - in: query
        name: StartTime
        description: The earliest scheduled start time to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - scheduled actions
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