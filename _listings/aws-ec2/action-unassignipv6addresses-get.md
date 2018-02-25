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
  /?Action=UnassignIpv6Addresses&k=1:
    get:
      summary: Unassign Ipv6 Addresses
      description: Unassigns one or more IPv6 addresses from a network interface
      operationId: unassignipv6addresses
      parameters:
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: PrivateIpAddress.N
        description: The secondary private IP addresses to unassign from the network
          interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - ipv6 addresses
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