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
  /?Action=DescribeImportSnapshotTasks&k=1:
    get:
      summary: Describe Import Snapshot Tasks
      description: Describes your import snapshot tasks
      operationId: describeimportsnapshottasks
      parameters:
      - in: query
        name: Description
        description: A description for the instance being imported
        type: string
      - in: query
        name: DiskImage.N
        description: The disk image
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      - in: query
        name: LaunchSpecification
        description: The launch specification
        type: string
      - in: query
        name: Platform
        description: The instance operating system
        type: string
      responses:
        200:
          description: OK
      tags:
      - import snapshot takss
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