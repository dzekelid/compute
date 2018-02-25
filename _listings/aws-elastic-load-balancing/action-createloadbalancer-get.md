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
  /?Action=CreateLoadBalancer&k=1:
    get:
      summary: ' Create Load Balancer '
      description: Creates an Application Load Balancer
      operationId: createLoadBalancer
      parameters:
      - in: query
        name: Name
        description: The name of the load balancer
        type: string
      - in: query
        name: Scheme
        description: The nodes of an Internet-facing load balancer have public IP
          addresses
        type: string
      - in: query
        name: SecurityGroups.member.N
        description: The IDs of the security groups to assign to the load balancer
        type: string
      - in: query
        name: Subnets.member.N
        description: The IDs of the subnets to attach to the load balancer
        type: string
      - in: query
        name: Tags.member.N
        description: One or more tags to assign to the load balancer
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