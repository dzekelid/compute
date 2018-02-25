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
  /?Action=DisassociateSubnetCidrBlock&k=1:
    get:
      summary: Disassociate Subnet Cidr Block
      description: Disassociates a CIDR block from a subnet
      operationId: disassociatesubnetcidrblock
      parameters:
      - in: query
        name: AssignIpv6AddressOnCreation
        description: Specify true to indicate that network interfaces created in the            specified
          subnet should be assigned an IPv6 address
        type: string
      - in: query
        name: MapPublicIpOnLaunch
        description: Specify true to indicate that network interfaces created in the            specified
          subnet should be assigned a public IPv4 address
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet
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