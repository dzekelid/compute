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
  /?Action=DeleteLoadBalancer&k=1:
    get:
      summary: ' Delete Load Balancer '
      description: Deletes the specified Application Load Balancer and its attached
        listeners
      operationId: deleteLoadBalancer
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - load balancers
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