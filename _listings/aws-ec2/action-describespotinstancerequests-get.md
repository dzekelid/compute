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
  /?Action=DescribeSpotInstanceRequests&k=1:
    get:
      summary: Describe Spot Instance Requests
      description: Describes the Spot instance requests that belong to your account
      operationId: describespotinstancerequests
      parameters:
      - in: query
        name: AvailabilityZone
        description: Filters the results by the specified Availability Zone
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EndTime
        description: The date and time, up to the current date, from which to stop
          retrieving the price history data,        in UTC format (for example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: InstanceType.N
        description: Filters the results by the specified instance types
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of results
        type: string
      - in: query
        name: ProductDescription.N
        description: Filters the results by the specified basic product descriptions
        type: string
      - in: query
        name: StartTime
        description: The date and time, up to the past 90 days, from which to start
          retrieving the price history data,        in UTC format (for example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      responses:
        200:
          description: OK
      tags:
      - spot instance requests
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