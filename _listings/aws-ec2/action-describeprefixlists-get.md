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
  /?Action=DescribePrefixLists&k=1:
    get:
      summary: Describe Prefix Lists
      description: Describes available AWS services in a prefix list format, which
        includes the prefix list name and prefix list ID of the service and the IP
        address range for the service
      operationId: describeprefixlists
      parameters:
      - in: query
        name: DryRun
        description: "Checks whether you have the required permissions for the action,
          without actually making the request, \t    and provides an error response"
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this request
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: VpcEndpointId.N
        description: One or more endpoint IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - prefix list
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