---
swagger: "2.0"
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeListeners&k=1:
    get:
      summary: ' Describe Listeners '
      description: Describes the specified listeners or the listeners for the specified
        Application Load Balancer
      operationId: describeListeners
      parameters:
      - in: query
        name: ListenerArns.member.N
        description: The Amazon Resource Names (ARN) of the listeners
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      responses:
        200:
          description: OK
      tags:
      - listeners
definitions: []
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