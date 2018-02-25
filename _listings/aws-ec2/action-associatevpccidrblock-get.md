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
  /?Action=AssociateVpcCidrBlock&k=1:
    get:
      summary: Associate Vpc Cidr Block
      description: Associates a CIDR block with your VPC
      operationId: associatevpccidrblock
      parameters:
      - in: query
        name: AmazonProvidedIpv6CidrBlock
        description: Requests an Amazon-provided IPv6 CIDR block with a /56 prefix
          length for the VPC
        type: string
      - in: query
        name: CidrBlock
        description: The IPv4 network range for the VPC, in CIDR notation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceTenancy
        description: The tenancy options for instances launched into the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - cidr block
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