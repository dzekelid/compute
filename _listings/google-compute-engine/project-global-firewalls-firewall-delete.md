---
swagger: "2.0"
info:
  title: Compute Engine
  description: Creates and runs virtual machines on Google Cloud Platform.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/firewalls/{firewall}:
    delete:
      summary: Delete Firewall
      description: Deletes the specified firewall
      operationId: compute.firewalls.delete
      parameters:
      - in: path
        name: firewall
        description: Name of the firewall rule to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - firewall
definitions:
  AccessConfig:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      natIP:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  Address:
    properties:
      address:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      users:
        description: This is a default description.
        type: parameters
  AddressAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  AddressList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  AddressesScopedList:
    properties:
      addresses:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  AttachedDisk:
    properties:
      autoDelete:
        description: This is a default description.
        type: parameters
      boot:
        description: This is a default description.
        type: parameters
      deviceName:
        description: This is a default description.
        type: parameters
      index:
        description: This is a default description.
        type: parameters
      interface:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      licenses:
        description: This is a default description.
        type: parameters
      mode:
        description: This is a default description.
        type: parameters
      source:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  AttachedDiskInitializeParams:
    properties:
      diskName:
        description: This is a default description.
        type: parameters
      diskSizeGb:
        description: This is a default description.
        type: parameters
      diskType:
        description: This is a default description.
        type: parameters
      sourceImage:
        description: This is a default description.
        type: parameters
  Autoscaler:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      target:
        description: This is a default description.
        type: parameters
      zone:
        description: This is a default description.
        type: parameters
  AutoscalerAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  AutoscalerList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  AutoscalersScopedList:
    properties:
      autoscalers:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  AutoscalingPolicy:
    properties:
      coolDownPeriodSec:
        description: This is a default description.
        type: parameters
      customMetricUtilizations:
        description: This is a default description.
        type: parameters
      maxNumReplicas:
        description: This is a default description.
        type: parameters
      minNumReplicas:
        description: This is a default description.
        type: parameters
  AutoscalingPolicyCpuUtilization:
    properties:
      utilizationTarget:
        description: This is a default description.
        type: parameters
  AutoscalingPolicyCustomMetricUtilization:
    properties:
      metric:
        description: This is a default description.
        type: parameters
      utilizationTarget:
        description: This is a default description.
        type: parameters
      utilizationTargetType:
        description: This is a default description.
        type: parameters
  AutoscalingPolicyLoadBalancingUtilization:
    properties:
      utilizationTarget:
        description: This is a default description.
        type: parameters
  Backend:
    properties:
      balancingMode:
        description: This is a default description.
        type: parameters
      capacityScaler:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      group:
        description: This is a default description.
        type: parameters
      maxConnections:
        description: This is a default description.
        type: parameters
      maxConnectionsPerInstance:
        description: This is a default description.
        type: parameters
      maxRate:
        description: This is a default description.
        type: parameters
      maxRatePerInstance:
        description: This is a default description.
        type: parameters
      maxUtilization:
        description: This is a default description.
        type: parameters
  BackendBucket:
    properties:
      bucketName:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      enableCdn:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  BackendBucketList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  BackendService:
    properties:
      affinityCookieTtlSec:
        description: This is a default description.
        type: parameters
      backends:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      enableCDN:
        description: This is a default description.
        type: parameters
      fingerprint:
        description: This is a default description.
        type: parameters
      healthChecks:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      loadBalancingScheme:
        description: This is a default description.
        type: parameters
  BackendServiceAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  BackendServiceGroupHealth:
    properties:
      healthStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  BackendServiceList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  BackendServicesScopedList:
    properties:
      backendServices:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  CacheInvalidationRule:
    properties:
      host:
        description: This is a default description.
        type: parameters
      path:
        description: This is a default description.
        type: parameters
  ConnectionDraining:
    properties:
      drainingTimeoutSec:
        description: This is a default description.
        type: parameters
  CustomerEncryptionKey:
    properties:
      rawKey:
        description: This is a default description.
        type: parameters
      sha256:
        description: This is a default description.
        type: parameters
  CustomerEncryptionKeyProtectedDisk:
    properties:
      source:
        description: This is a default description.
        type: parameters
  DeprecationStatus:
    properties:
      deleted:
        description: This is a default description.
        type: parameters
      deprecated:
        description: This is a default description.
        type: parameters
      obsolete:
        description: This is a default description.
        type: parameters
      replacement:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
  Disk:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      lastAttachTimestamp:
        description: This is a default description.
        type: parameters
      lastDetachTimestamp:
        description: This is a default description.
        type: parameters
      licenses:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      options:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  DiskAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  DiskList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  DiskMoveRequest:
    properties:
      destinationZone:
        description: This is a default description.
        type: parameters
      targetDisk:
        description: This is a default description.
        type: parameters
  DiskType:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      defaultDiskSizeGb:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      validDiskSize:
        description: This is a default description.
        type: parameters
      zone:
        description: This is a default description.
        type: parameters
  DiskTypeAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  DiskTypeList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  DiskTypesScopedList:
    properties:
      diskTypes:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  DisksResizeRequest:
    properties:
      sizeGb:
        description: This is a default description.
        type: parameters
  DisksScopedList:
    properties:
      disks:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  Firewall:
    properties:
      allowed:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      sourceRanges:
        description: This is a default description.
        type: parameters
      sourceTags:
        description: This is a default description.
        type: parameters
  FirewallList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  ForwardingRule:
    properties:
      IPAddress:
        description: This is a default description.
        type: parameters
      IPProtocol:
        description: This is a default description.
        type: parameters
      backendService:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      loadBalancingScheme:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
  ForwardingRuleAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  ForwardingRuleList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  ForwardingRulesScopedList:
    properties:
      forwardingRules:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  GuestOsFeature:
    properties:
      type:
        description: This is a default description.
        type: parameters
  HTTPHealthCheck:
    properties:
      host:
        description: This is a default description.
        type: parameters
      port:
        description: This is a default description.
        type: parameters
      portName:
        description: This is a default description.
        type: parameters
      proxyHeader:
        description: This is a default description.
        type: parameters
      requestPath:
        description: This is a default description.
        type: parameters
      checkIntervalSec:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      healthyThreshold:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
  HTTPSHealthCheck:
    properties:
      host:
        description: This is a default description.
        type: parameters
      port:
        description: This is a default description.
        type: parameters
      portName:
        description: This is a default description.
        type: parameters
      proxyHeader:
        description: This is a default description.
        type: parameters
      requestPath:
        description: This is a default description.
        type: parameters
      checkIntervalSec:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      healthyThreshold:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
  HealthCheck:
    properties:
      checkIntervalSec:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      healthyThreshold:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      timeoutSec:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  HealthCheckList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  HealthCheckReference:
    properties:
      healthCheck:
        description: This is a default description.
        type: parameters
  HealthStatus:
    properties:
      healthState:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      ipAddress:
        description: This is a default description.
        type: parameters
      port:
        description: This is a default description.
        type: parameters
  HostRule:
    properties:
      description:
        description: This is a default description.
        type: parameters
      hosts:
        description: This is a default description.
        type: parameters
      pathMatcher:
        description: This is a default description.
        type: parameters
  HttpHealthCheckList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  HttpsHealthCheckList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Image:
    properties:
      archiveSizeBytes:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      diskSizeGb:
        description: This is a default description.
        type: parameters
      family:
        description: This is a default description.
        type: parameters
      guestOsFeatures:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      licenses:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  ImageList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Instance:
    properties:
      canIpForward:
        description: This is a default description.
        type: parameters
      cpuPlatform:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      disks:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      machineType:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      networkInterfaces:
        description: This is a default description.
        type: parameters
  InstanceAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroup:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      fingerprint:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      namedPorts:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroupAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroupList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroupManager:
    properties:
      baseInstanceName:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      fingerprint:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      instanceGroup:
        description: This is a default description.
        type: parameters
      instanceTemplate:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      namedPorts:
        description: This is a default description.
        type: parameters
  InstanceGroupManagerActionsSummary:
    properties:
      abandoning:
        description: This is a default description.
        type: parameters
      creating:
        description: This is a default description.
        type: parameters
      creatingWithoutRetries:
        description: This is a default description.
        type: parameters
      deleting:
        description: This is a default description.
        type: parameters
      none:
        description: This is a default description.
        type: parameters
      recreating:
        description: This is a default description.
        type: parameters
      refreshing:
        description: This is a default description.
        type: parameters
      restarting:
        description: This is a default description.
        type: parameters
  InstanceGroupManagerAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroupManagerList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersAbandonInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersDeleteInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersListManagedInstancesResponse:
    properties:
      managedInstances:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersRecreateInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersScopedList:
    properties:
      instanceGroupManagers:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersSetInstanceTemplateRequest:
    properties:
      instanceTemplate:
        description: This is a default description.
        type: parameters
  InstanceGroupManagersSetTargetPoolsRequest:
    properties:
      fingerprint:
        description: This is a default description.
        type: parameters
      targetPools:
        description: This is a default description.
        type: parameters
  InstanceGroupsAddInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  InstanceGroupsListInstances:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceGroupsListInstancesRequest:
    properties:
      instanceState:
        description: This is a default description.
        type: parameters
  InstanceGroupsRemoveInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  InstanceGroupsScopedList:
    properties:
      instanceGroups:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  InstanceGroupsSetNamedPortsRequest:
    properties:
      fingerprint:
        description: This is a default description.
        type: parameters
      namedPorts:
        description: This is a default description.
        type: parameters
  InstanceList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceMoveRequest:
    properties:
      destinationZone:
        description: This is a default description.
        type: parameters
      targetInstance:
        description: This is a default description.
        type: parameters
  InstanceProperties:
    properties:
      canIpForward:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      disks:
        description: This is a default description.
        type: parameters
      machineType:
        description: This is a default description.
        type: parameters
      networkInterfaces:
        description: This is a default description.
        type: parameters
      serviceAccounts:
        description: This is a default description.
        type: parameters
  InstanceReference:
    properties:
      instance:
        description: This is a default description.
        type: parameters
  InstanceTemplate:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceTemplateList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  InstanceWithNamedPorts:
    properties:
      instance:
        description: This is a default description.
        type: parameters
      namedPorts:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  InstancesScopedList:
    properties:
      instances:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  InstancesSetMachineTypeRequest:
    properties:
      machineType:
        description: This is a default description.
        type: parameters
  InstancesSetServiceAccountRequest:
    properties:
      email:
        description: This is a default description.
        type: parameters
      scopes:
        description: This is a default description.
        type: parameters
  InstancesStartWithEncryptionKeyRequest:
    properties:
      disks:
        description: This is a default description.
        type: parameters
  License:
    properties:
      chargesUseFee:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  MachineType:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      guestCpus:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      imageSpaceGb:
        description: This is a default description.
        type: parameters
      isSharedCpu:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      maximumPersistentDisks:
        description: This is a default description.
        type: parameters
      maximumPersistentDisksSizeGb:
        description: This is a default description.
        type: parameters
      memoryMb:
        description: This is a default description.
        type: parameters
  MachineTypeAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  MachineTypeList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  MachineTypesScopedList:
    properties:
      machineTypes:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  ManagedInstance:
    properties:
      currentAction:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      instanceStatus:
        description: This is a default description.
        type: parameters
  ManagedInstanceLastAttempt:
    properties:
      errors:
        description: This is a default description.
        type: parameters
  Metadata:
    properties:
      fingerprint:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  NamedPort:
    properties:
      name:
        description: This is a default description.
        type: parameters
      port:
        description: This is a default description.
        type: parameters
  Network:
    properties:
      IPv4Range:
        description: This is a default description.
        type: parameters
      autoCreateSubnetworks:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      gatewayIPv4:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      subnetworks:
        description: This is a default description.
        type: parameters
  NetworkInterface:
    properties:
      accessConfigs:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      networkIP:
        description: This is a default description.
        type: parameters
      subnetwork:
        description: This is a default description.
        type: parameters
  NetworkList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Operation:
    properties:
      clientOperationId:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      endTime:
        description: This is a default description.
        type: parameters
      error:
        description: This is a default description.
        type: parameters
      httpErrorMessage:
        description: This is a default description.
        type: parameters
      httpErrorStatusCode:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      insertTime:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OperationAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  OperationList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  OperationsScopedList:
    properties:
      operations:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  PathMatcher:
    properties:
      defaultService:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      pathRules:
        description: This is a default description.
        type: parameters
  PathRule:
    properties:
      paths:
        description: This is a default description.
        type: parameters
      service:
        description: This is a default description.
        type: parameters
  Project:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      defaultServiceAccount:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      enabledFeatures:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      quotas:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Quota:
    properties:
      limit:
        description: This is a default description.
        type: parameters
      metric:
        description: This is a default description.
        type: parameters
      usage:
        description: This is a default description.
        type: parameters
  Region:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      quotas:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      zones:
        description: This is a default description.
        type: parameters
  RegionAutoscalerList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagerList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagersAbandonInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagersDeleteInstancesRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagersListInstancesResponse:
    properties:
      managedInstances:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagersRecreateRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagersSetTargetPoolsRequest:
    properties:
      fingerprint:
        description: This is a default description.
        type: parameters
      targetPools:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupManagersSetTemplateRequest:
    properties:
      instanceTemplate:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupsListInstances:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupsListInstancesRequest:
    properties:
      instanceState:
        description: This is a default description.
        type: parameters
      portName:
        description: This is a default description.
        type: parameters
  RegionInstanceGroupsSetNamedPortsRequest:
    properties:
      fingerprint:
        description: This is a default description.
        type: parameters
      namedPorts:
        description: This is a default description.
        type: parameters
  RegionList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  ResourceGroupReference:
    properties:
      group:
        description: This is a default description.
        type: parameters
  Route:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      destRange:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      nextHopGateway:
        description: This is a default description.
        type: parameters
      nextHopInstance:
        description: This is a default description.
        type: parameters
      nextHopIp:
        description: This is a default description.
        type: parameters
  RouteList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Router:
    properties:
      bgpPeers:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      interfaces:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RouterAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RouterBgp:
    properties:
      asn:
        description: This is a default description.
        type: parameters
  RouterBgpPeer:
    properties:
      advertisedRoutePriority:
        description: This is a default description.
        type: parameters
      interfaceName:
        description: This is a default description.
        type: parameters
      ipAddress:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      peerAsn:
        description: This is a default description.
        type: parameters
      peerIpAddress:
        description: This is a default description.
        type: parameters
  RouterInterface:
    properties:
      ipRange:
        description: This is a default description.
        type: parameters
      linkedVpnTunnel:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  RouterList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  RouterStatus:
    properties:
      bestRoutes:
        description: This is a default description.
        type: parameters
      bgpPeerStatus:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
  RouterStatusBgpPeerStatus:
    properties:
      advertisedRoutes:
        description: This is a default description.
        type: parameters
      ipAddress:
        description: This is a default description.
        type: parameters
      linkedVpnTunnel:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      numLearnedRoutes:
        description: This is a default description.
        type: parameters
      peerIpAddress:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      uptime:
        description: This is a default description.
        type: parameters
      uptimeSeconds:
        description: This is a default description.
        type: parameters
  RouterStatusResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  RoutersPreviewResponse:
    properties: []
  RoutersScopedList:
    properties:
      routers:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  SSLHealthCheck:
    properties:
      port:
        description: This is a default description.
        type: parameters
      portName:
        description: This is a default description.
        type: parameters
      proxyHeader:
        description: This is a default description.
        type: parameters
      request:
        description: This is a default description.
        type: parameters
      response:
        description: This is a default description.
        type: parameters
  Scheduling:
    properties:
      automaticRestart:
        description: This is a default description.
        type: parameters
      onHostMaintenance:
        description: This is a default description.
        type: parameters
      preemptible:
        description: This is a default description.
        type: parameters
  SerialPortOutput:
    properties:
      contents:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      next:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      start:
        description: This is a default description.
        type: parameters
  ServiceAccount:
    properties:
      email:
        description: This is a default description.
        type: parameters
      scopes:
        description: This is a default description.
        type: parameters
  Snapshot:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      diskSizeGb:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      licenses:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      sourceDisk:
        description: This is a default description.
        type: parameters
      sourceDiskId:
        description: This is a default description.
        type: parameters
  SnapshotList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  SslCertificate:
    properties:
      certificate:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      privateKey:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  SslCertificateList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Subnetwork:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      gatewayAddress:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      ipCidrRange:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  SubnetworkAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  SubnetworkList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  SubnetworksExpandIpCidrRangeRequest:
    properties:
      ipCidrRange:
        description: This is a default description.
        type: parameters
  SubnetworksScopedList:
    properties:
      subnetworks:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  TCPHealthCheck:
    properties:
      port:
        description: This is a default description.
        type: parameters
      portName:
        description: This is a default description.
        type: parameters
      proxyHeader:
        description: This is a default description.
        type: parameters
      request:
        description: This is a default description.
        type: parameters
      response:
        description: This is a default description.
        type: parameters
  Tags:
    properties:
      fingerprint:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
  TargetHttpProxy:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      urlMap:
        description: This is a default description.
        type: parameters
  TargetHttpProxyList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetHttpsProxiesSetSslCertificatesRequest:
    properties:
      sslCertificates:
        description: This is a default description.
        type: parameters
  TargetHttpsProxy:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      sslCertificates:
        description: This is a default description.
        type: parameters
      urlMap:
        description: This is a default description.
        type: parameters
  TargetHttpsProxyList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetInstance:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      natPolicy:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      zone:
        description: This is a default description.
        type: parameters
  TargetInstanceAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetInstanceList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetInstancesScopedList:
    properties:
      targetInstances:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  TargetPool:
    properties:
      backupPool:
        description: This is a default description.
        type: parameters
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      failoverRatio:
        description: This is a default description.
        type: parameters
      healthChecks:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      instances:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
  TargetPoolAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetPoolInstanceHealth:
    properties:
      healthStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  TargetPoolList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetPoolsAddHealthCheckRequest:
    properties:
      healthChecks:
        description: This is a default description.
        type: parameters
  TargetPoolsAddInstanceRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  TargetPoolsRemoveHealthCheckRequest:
    properties:
      healthChecks:
        description: This is a default description.
        type: parameters
  TargetPoolsRemoveInstanceRequest:
    properties:
      instances:
        description: This is a default description.
        type: parameters
  TargetPoolsScopedList:
    properties:
      targetPools:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  TargetReference:
    properties:
      target:
        description: This is a default description.
        type: parameters
  TargetSslProxiesSetBackendServiceRequest:
    properties:
      service:
        description: This is a default description.
        type: parameters
  TargetSslProxiesSetProxyHeaderRequest:
    properties:
      proxyHeader:
        description: This is a default description.
        type: parameters
  TargetSslProxiesSetSslCertificatesRequest:
    properties:
      sslCertificates:
        description: This is a default description.
        type: parameters
  TargetSslProxy:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      proxyHeader:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      service:
        description: This is a default description.
        type: parameters
      sslCertificates:
        description: This is a default description.
        type: parameters
  TargetSslProxyList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetVpnGateway:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      forwardingRules:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      network:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  TargetVpnGatewayAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetVpnGatewayList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  TargetVpnGatewaysScopedList:
    properties:
      targetVpnGateways:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  TestFailure:
    properties:
      actualService:
        description: This is a default description.
        type: parameters
      expectedService:
        description: This is a default description.
        type: parameters
      host:
        description: This is a default description.
        type: parameters
      path:
        description: This is a default description.
        type: parameters
  UrlMap:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      defaultService:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      fingerprint:
        description: This is a default description.
        type: parameters
      hostRules:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      pathMatchers:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  UrlMapList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  UrlMapReference:
    properties:
      urlMap:
        description: This is a default description.
        type: parameters
  UrlMapTest:
    properties:
      description:
        description: This is a default description.
        type: parameters
      host:
        description: This is a default description.
        type: parameters
      path:
        description: This is a default description.
        type: parameters
      service:
        description: This is a default description.
        type: parameters
  UrlMapValidationResult:
    properties:
      loadErrors:
        description: This is a default description.
        type: parameters
      loadSucceeded:
        description: This is a default description.
        type: parameters
      testFailures:
        description: This is a default description.
        type: parameters
      testPassed:
        description: This is a default description.
        type: parameters
  UrlMapsValidateRequest:
    properties: []
  UrlMapsValidateResponse:
    properties: []
  UsageExportLocation:
    properties:
      bucketName:
        description: This is a default description.
        type: parameters
      reportNamePrefix:
        description: This is a default description.
        type: parameters
  VpnTunnel:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      detailedStatus:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      ikeVersion:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      localTrafficSelector:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      peerIp:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
  VpnTunnelAggregatedList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  VpnTunnelList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  VpnTunnelsScopedList:
    properties:
      vpnTunnels:
        description: This is a default description.
        type: parameters
      warning:
        description: This is a default description.
        type: parameters
  Zone:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  ZoneList:
    properties:
      id:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
x-collection-name: Google Compute Engine
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