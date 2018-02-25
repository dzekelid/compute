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
  /?Action=DescribeSecurityGroupReferences (EC2-VPC only)&k=1:
    get:
      summary: Describe Security Group References ( E C2- V P C only)
      description: '[EC2-VPC only] Describes the VPCs on the other side of a VPC peering
        connection that are referencing the security groups you''ve specified in this
        request'
      operationId: describesecuritygroupreferences-ec2vpc-only
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: GroupId.N
        description: One or more security group IDs
        type: string
      - in: query
        name: GroupName.N
        description: '[EC2-Classic and default VPC only] One or more security group
          names'
        type: string
      responses:
        200:
          description: OK
      tags:
      - security group
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