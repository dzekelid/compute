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
  /?Action=ModifyHosts&k=1:
    get:
      summary: Modify Hosts
      description: Modify the auto-placement setting of a Dedicated Host
      operationId: modifyhosts
      parameters:
      - in: query
        name: Affinity
        description: The new affinity setting for the instance
        type: string
      - in: query
        name: HostId
        description: The ID of the Dedicated Host that the instance will have affinity
          with
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance that you are modifying
        type: string
      - in: query
        name: Tenancy
        description: The tenancy of the instance that you are modifying
        type: string
      responses:
        200:
          description: OK
      tags:
      - hosts
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