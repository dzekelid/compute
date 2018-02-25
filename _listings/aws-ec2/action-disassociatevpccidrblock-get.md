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
  /?Action=DisassociateVpcCidrBlock&k=1:
    get:
      summary: Disassociate Vpc Cidr Block
      description: Disassociates a CIDR block from a VPC
      operationId: disassociatevpccidrblock
      parameters:
      - in: query
        name: EnableDnsHostnames
        description: Indicates whether the instances launched in the VPC get DNS hostnames
        type: string
      - in: query
        name: EnableDnsSupport
        description: Indicates whether the DNS resolution is supported for the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
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