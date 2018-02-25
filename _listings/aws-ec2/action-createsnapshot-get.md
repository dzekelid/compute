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
  /?Action=CreateSnapshot&k=1:
    get:
      summary: Create Snapshot
      description: Creates a snapshot of an EBS volume and stores it in Amazon S3
      operationId: createsnapshot
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone in which to create the volume
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the volume should be encrypted
        type: string
      - in: query
        name: Iops
        description: Only valid for Provisioned IOPS SSD volumes
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) customer
          master key (CMK) to use when creating the encrypted      volume
        type: string
      - in: query
        name: Size
        description: The size of the volume, in GiBs
        type: string
      - in: query
        name: SnapshotId
        description: The snapshot from which to create the volume
        type: string
      - in: query
        name: VolumeType
        description: The volume type
        type: string
      responses:
        200:
          description: OK
      tags:
      - snapshot
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