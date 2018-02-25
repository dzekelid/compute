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
  /?Action=RequestSpotFleet&k=1:
    get:
      summary: Request Spot Fleet
      description: Creates a Spot fleet request
      operationId: requestspotfleet
      parameters:
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 CIDR block for your subnet
        type: string
      - in: query
        name: SubnetId
        description: The ID of your subnet
        type: string
      responses:
        200:
          description: OK
      tags:
      - spot fleet
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