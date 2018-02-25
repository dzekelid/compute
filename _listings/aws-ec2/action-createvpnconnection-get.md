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
  /?Action=CreateVpnConnection&k=1:
    get:
      summary: Create Vpn Connection
      description: |-
        Creates a VPN connection between an existing virtual private gateway and a VPN customer
                    gateway
      operationId: createvpnconnection
      parameters:
      - in: query
        name: DestinationCidrBlock
        description: The CIDR block associated with the local subnet of the customer
          network
        type: string
      - in: query
        name: VpnConnectionId
        description: The ID of the VPN connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - vpc connection
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