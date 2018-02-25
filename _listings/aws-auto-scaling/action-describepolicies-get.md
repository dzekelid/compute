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
  /?Action=DescribePolicies&k=1:
    get:
      summary: ' Describe Policies '
      description: Describes the policies for the specified Auto Scaling group
      operationId: describePolicies
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to be returned with each call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: PolicyNames.member.N
        description: One or more policy names or policy ARNs to be described
        type: string
      - in: query
        name: PolicyTypes.member.N
        description: One or more policy types
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