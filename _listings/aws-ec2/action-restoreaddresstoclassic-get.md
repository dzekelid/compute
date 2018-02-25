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
  /?Action=RestoreAddressToClassic&k=1:
    get:
      summary: Restore Address To Classic
      description: Restores an Elastic IP address that was previously moved to the
        EC2-VPC platform back to the EC2-Classic platform
      operationId: restoreaddresstoclassic
      parameters:
      - in: query
        name: Ipv6AddressCount
        description: The number of IPv6 addresses to assign to the network interface
        type: string
      - in: query
        name: Ipv6Addresses.N
        description: One or more specific IPv6 addresses to be assigned to the network
          interface
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - ip address
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