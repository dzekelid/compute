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
  /?Action=AllocateAddress&k=1:
    get:
      summary: Allocate Address
      description: Acquires an Elastic IP address
      operationId: allocateaddress
      parameters:
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: AllowReassociation
        description: '[EC2-VPC] For a VPC in an EC2-Classic account, specify true
          to allow an Elastic IP address that is already associated with an instance
          or network interface to be reassociated with the specified instance or network
          interface'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: NetworkInterfaceId
        description: '[EC2-VPC] The ID of the network interface'
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary or secondary private IP address to associate
          with the Elastic IP address'
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
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