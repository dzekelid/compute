---
swagger: "2.0"
info:
  title: Reverse DNS API
  description: Use the reverse DNS API operations to view and manage the PTR records
    associated with a Rackspace cloud device.
  version: 1.0.0
host: global.dns.api.rackspacecloud.com
basePath: /v2/{tenant_id}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? |
    /v1.0/{account}/rdns/{service-name}/{recordId}
  : get:
      summary: Show PTR record
      description: |-
        This call shows details for a specified PTR record associated with a specified
        cloud device
      operationId: show-ptr-record
      parameters:
      - in: header
        name: "200"
        description: Request succeeded
        type: <td>success</td>
      - in: header
        name: "400"
        description: The request is missingone or more elements, orthe values of someelements
          are invalid
        type: <td>bad request</td>
      - in: header
        name: 400 500
        description: The DNS service hasexperienced a fault
        type: <td>dnsfault</td>
      - in: header
        name: "401"
        description: You are not authorizedto complete thisoperation
        type: <td>unauthorized</td>
      - in: header
        name: "404"
        description: The requested item wasnot found
        type: <td>not found</td>
      - in: header
        name: "413"
        description: The number of itemsreturned is above theallowed limit
        type: <td>over limit</td>
      - in: header
        name: "503"
        description: The service is notavailable
        type: <td>service unavailable</td>
      - in: query
        name: account
        description: The tenant ID
        type: <td>string</td>
      - in: query
        name: recordId
        description: ID for the record
        type: <td>string</td>
      - in: query
        name: service-name
        description: Name of the Cloudservice
        type: <td>string</td>
      responses:
        200:
          description: OK
      tags:
      - reverse dns
definitions: []
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