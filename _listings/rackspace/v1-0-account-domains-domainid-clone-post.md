---
swagger: "2.0"
info:
  title: DNS Domains API
  description: Use the Domains operations to view and manage domains and subdomains
    for a Rackspace Cloud account.
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
    /v1.0/{account}/domains/{domainId}/clone
  : post:
      summary: Clone domain
      description: Creates a specified domain ( example2
      operationId: clone-domain
      parameters:
      - in: query
        name: account
        description: The tenant ID
        type: <td>string</td>
      - in: query
        name: domainId
        description: ID for the domain
        type: <td>string</td>
      responses:
        200:
          description: OK
      tags:
      - domains
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