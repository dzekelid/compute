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
  /?Action=UpdateAutoScalingGroup&k=1:
    get:
      summary: ' Update Auto Scaling Group '
      description: Updates the configuration for the specified Auto Scaling group
      operationId: updateAutoScalingGroup
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: AvailabilityZones.member.N
        description: One or more Availability Zones for the group
        type: string
      - in: query
        name: DefaultCooldown
        description: The amount of time, in seconds, after a scaling activity completes
          before another scaling activity can start
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the Auto
          Scaling group
        type: string
      - in: query
        name: HealthCheckGracePeriod
        description: The amount of time, in seconds, that Auto Scaling waits before
          checking the health status of an EC2 instance that has come into service
        type: string
      - in: query
        name: HealthCheckType
        description: The service to use for the health checks
        type: string
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      - in: query
        name: MaxSize
        description: The maximum size of the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size of the Auto Scaling group
        type: string
      - in: query
        name: NewInstancesProtectedFromScaleIn
        description: Indicates whether newly launched instances are protected from
          termination by Auto Scaling when scaling in
        type: string
      - in: query
        name: PlacementGroup
        description: The name of the placement group into which you'll launch your
          instances, if any
        type: string
      - in: query
        name: TerminationPolicies.member.N
        description: A standalone termination policy or a list of termination policies
          used to select the instance to terminate
        type: string
      - in: query
        name: VPCZoneIdentifier
        description: The ID of the subnet, if you are launching into a VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - auto scaling
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