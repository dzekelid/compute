---
swagger: "2.0"
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResumeProcesses&k=1:
    get:
      summary: ' Resume Processes '
      description: Resumes the specified suspended Auto Scaling processes, or all
        suspended process, for the specified Auto Scaling group
      operationId: resumeProcesses
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: ScalingProcesses.member.N
        description: One or more of the following processes
        type: string
      responses:
        200:
          description: OK
      tags:
      - processes
definitions: []
x-collection-name: AWS Auto Scaling
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