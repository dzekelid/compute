---
swagger: "2.0"
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteComputeEnvironment:
    get:
      summary: ' Delete Compute Environment '
      description: Deletes an AWS Batch compute environment
      operationId: deleteComputeEnvironment
      parameters:
      - in: query
        name: computeEnvironment
        description: The name or Amazon Resource Name (ARN) of the compute environment
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - compute environment
definitions: []
x-collection-name: AWS Batch
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