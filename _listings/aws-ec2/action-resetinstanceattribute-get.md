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
  /?Action=ResetInstanceAttribute&k=1:
    get:
      summary: Reset Instance Attribute
      description: Resets an attribute of an instance to its default value
      operationId: resetinstanceattribute
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: BlockDeviceMapping.N
        description: The block device mapping
        type: string
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DisableApiTermination
        description: If you set this parameter to true, you can't terminate the instance            using
          the Amazon EC2 console, CLI, or API; otherwise, you can
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EbsOptimized
        description: Indicates whether the instance is optimized for EBS I/O
        type: string
      - in: query
        name: IamInstanceProfile
        description: The IAM instance profile
        type: string
      - in: query
        name: ImageId
        description: The ID of the AMI, which you can get by calling DescribeImages
        type: string
      - in: query
        name: InstanceInitiatedShutdownBehavior
        description: Indicates whether an instance stops or terminates when you initiate
          shutdown from the instance (using the operating system command for system
          shutdown)
        type: string
      - in: query
        name: InstanceType
        description: The instance type
        type: string
      - in: query
        name: Ipv6Address.N
        description: '[EC2-VPC] Specify one or more IPv6 addresses from the range
          of the subnet to            associate with the primary network interface'
        type: string
      - in: query
        name: Ipv6AddressCount
        description: '[EC2-VPC] A number of IPv6 addresses to associate with the primary
          network            interface'
        type: string
      - in: query
        name: KernelId
        description: The ID of the kernel
        type: string
      - in: query
        name: KeyName
        description: The name of the key pair
        type: string
      - in: query
        name: MaxCount
        description: The maximum number of instances to launch
        type: string
      - in: query
        name: MinCount
        description: The minimum number of instances to launch
        type: string
      - in: query
        name: Monitoring
        description: The monitoring for the instance
        type: string
      - in: query
        name: NetworkInterface.N
        description: One or more network interfaces
        type: string
      - in: query
        name: Placement
        description: The placement for the instance
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary IPv4 address'
        type: string
      - in: query
        name: RamdiskId
        description: The ID of the RAM disk
        type: string
      - in: query
        name: SecurityGroup.N
        description: '[EC2-Classic, default VPC] One or more security group names'
        type: string
      - in: query
        name: SecurityGroupId.N
        description: One or more security group IDs
        type: string
      - in: query
        name: SubnetId
        description: '[EC2-VPC] The ID of the subnet to launch the instance into'
        type: string
      - in: query
        name: UserData
        description: The user data to make available to the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - server instance
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