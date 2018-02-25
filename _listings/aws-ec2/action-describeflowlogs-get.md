---
swagger: "2.0"
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeFlowLogs&k=1:
    get:
      summary: Describe Flow Logs
      description: Describes one or more flow logs
      operationId: describeflowlogs
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DryRun
        description: "Checks whether you have the required permissions for the action,
          without actually making the request, \t    and provides an error response"
        type: string
      - in: query
        name: PolicyDocument
        description: A policy to attach to the endpoint that controls access to the
          service
        type: string
      - in: query
        name: RouteTableId.N
        description: One or more route table IDs
        type: string
      - in: query
        name: ServiceName
        description: The AWS service name, in the form com
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC in which the endpoint will be used
        type: string
      responses:
        200:
          description: OK
      tags:
      - flow logs
definitions: []
x-collection-name: AWS EC2
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