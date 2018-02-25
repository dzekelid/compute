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
  /?Action=SetSubnets&k=1:
    get:
      summary: ' Set Subnets '
      description: Enables the Availability Zone for the specified subnets for the
        specified load balancer
      operationId: setSubnets
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Subnets.member.N
        description: The IDs of the subnets
        type: string
      responses:
        200:
          description: OK
      tags:
      - subnets
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