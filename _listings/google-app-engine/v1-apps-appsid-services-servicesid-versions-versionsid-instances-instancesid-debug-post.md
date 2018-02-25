---
swagger: "2.0"
info:
  title: Google App Engine Admin
  description: Provisions and manages App Engine applications.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: appengine.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/apps/{appsId}/services/{servicesId}/versions/{versionsId}/instances/{instancesId}:debug:
    post:
      summary: Enable Debugging
      description: Enables debugging on a VM instance
      operationId: appengine.apps.services.versions.instances.debug
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instancesId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - debugging
definitions:
  ApiConfigHandler:
    properties:
      authFailAction:
        description: This is a default description.
        type: post
      login:
        description: This is a default description.
        type: post
      script:
        description: This is a default description.
        type: post
      securityLevel:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  ApiEndpointHandler:
    properties:
      scriptPath:
        description: This is a default description.
        type: post
  Application:
    properties:
      authDomain:
        description: This is a default description.
        type: post
      codeBucket:
        description: This is a default description.
        type: post
      defaultBucket:
        description: This is a default description.
        type: post
      defaultCookieExpiration:
        description: This is a default description.
        type: post
      defaultHostname:
        description: This is a default description.
        type: post
      dispatchRules:
        description: This is a default description.
        type: post
      gcrDomain:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      locationId:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  AutomaticScaling:
    properties:
      coolDownPeriod:
        description: This is a default description.
        type: post
      maxConcurrentRequests:
        description: This is a default description.
        type: post
      maxIdleInstances:
        description: This is a default description.
        type: post
      maxPendingLatency:
        description: This is a default description.
        type: post
      maxTotalInstances:
        description: This is a default description.
        type: post
      minIdleInstances:
        description: This is a default description.
        type: post
      minPendingLatency:
        description: This is a default description.
        type: post
      minTotalInstances:
        description: This is a default description.
        type: post
  BasicScaling:
    properties:
      idleTimeout:
        description: This is a default description.
        type: post
      maxInstances:
        description: This is a default description.
        type: post
  ContainerInfo:
    properties:
      image:
        description: This is a default description.
        type: post
  CpuUtilization:
    properties:
      aggregationWindowLength:
        description: This is a default description.
        type: post
      targetUtilization:
        description: This is a default description.
        type: post
  DebugInstanceRequest:
    properties:
      sshKey:
        description: This is a default description.
        type: post
  Deployment:
    properties:
      files:
        description: This is a default description.
        type: post
  DiskUtilization:
    properties:
      targetReadBytesPerSecond:
        description: This is a default description.
        type: post
      targetReadOpsPerSecond:
        description: This is a default description.
        type: post
      targetWriteBytesPerSecond:
        description: This is a default description.
        type: post
      targetWriteOpsPerSecond:
        description: This is a default description.
        type: post
  EndpointsApiService:
    properties:
      configId:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  ErrorHandler:
    properties:
      errorCode:
        description: This is a default description.
        type: post
      mimeType:
        description: This is a default description.
        type: post
      staticFile:
        description: This is a default description.
        type: post
  FileInfo:
    properties:
      mimeType:
        description: This is a default description.
        type: post
      sha1Sum:
        description: This is a default description.
        type: post
      sourceUrl:
        description: This is a default description.
        type: post
  HealthCheck:
    properties:
      checkInterval:
        description: This is a default description.
        type: post
      disableHealthCheck:
        description: This is a default description.
        type: post
      healthyThreshold:
        description: This is a default description.
        type: post
      host:
        description: This is a default description.
        type: post
      restartThreshold:
        description: This is a default description.
        type: post
      timeout:
        description: This is a default description.
        type: post
      unhealthyThreshold:
        description: This is a default description.
        type: post
  IdentityAwareProxy:
    properties:
      enabled:
        description: This is a default description.
        type: post
      oauth2ClientId:
        description: This is a default description.
        type: post
      oauth2ClientSecret:
        description: This is a default description.
        type: post
      oauth2ClientSecretSha256:
        description: This is a default description.
        type: post
  Instance:
    properties:
      appEngineRelease:
        description: This is a default description.
        type: post
      availability:
        description: This is a default description.
        type: post
      averageLatency:
        description: This is a default description.
        type: post
      errors:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      memoryUsage:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      qps:
        description: This is a default description.
        type: post
      requests:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
  Library:
    properties:
      name:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  ListInstancesResponse:
    properties:
      instances:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  ListLocationsResponse:
    properties:
      locations:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      operations:
        description: This is a default description.
        type: post
  ListServicesResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      services:
        description: This is a default description.
        type: post
  ListVersionsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      versions:
        description: This is a default description.
        type: post
  LivenessCheck:
    properties:
      checkInterval:
        description: This is a default description.
        type: post
      healthyThreshold:
        description: This is a default description.
        type: post
      host:
        description: This is a default description.
        type: post
      initialDelay:
        description: This is a default description.
        type: post
      path:
        description: This is a default description.
        type: post
      timeout:
        description: This is a default description.
        type: post
      unhealthyThreshold:
        description: This is a default description.
        type: post
  Location:
    properties:
      labels:
        description: This is a default description.
        type: post
      locationId:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  LocationMetadata:
    properties:
      flexibleEnvironmentAvailable:
        description: This is a default description.
        type: post
      standardEnvironmentAvailable:
        description: This is a default description.
        type: post
  ManualScaling:
    properties:
      instances:
        description: This is a default description.
        type: post
  Network:
    properties:
      forwardedPorts:
        description: This is a default description.
        type: post
      instanceTag:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      subnetworkName:
        description: This is a default description.
        type: post
  NetworkUtilization:
    properties:
      targetReceivedBytesPerSecond:
        description: This is a default description.
        type: post
      targetReceivedPacketsPerSecond:
        description: This is a default description.
        type: post
      targetSentBytesPerSecond:
        description: This is a default description.
        type: post
      targetSentPacketsPerSecond:
        description: This is a default description.
        type: post
  Operation:
    properties:
      done:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      response:
        description: This is a default description.
        type: post
  OperationMetadata:
    properties:
      endTime:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      method:
        description: This is a default description.
        type: post
      operationType:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      user:
        description: This is a default description.
        type: post
  OperationMetadataExperimental:
    properties:
      endTime:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      method:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      user:
        description: This is a default description.
        type: post
  OperationMetadataV1:
    properties:
      endTime:
        description: This is a default description.
        type: post
      ephemeralMessage:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      method:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      user:
        description: This is a default description.
        type: post
      warning:
        description: This is a default description.
        type: post
  OperationMetadataV1Alpha:
    properties:
      endTime:
        description: This is a default description.
        type: post
      ephemeralMessage:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      method:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      user:
        description: This is a default description.
        type: post
      warning:
        description: This is a default description.
        type: post
  OperationMetadataV1Beta:
    properties:
      endTime:
        description: This is a default description.
        type: post
      ephemeralMessage:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      method:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      user:
        description: This is a default description.
        type: post
      warning:
        description: This is a default description.
        type: post
  OperationMetadataV1Beta5:
    properties:
      endTime:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      method:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      user:
        description: This is a default description.
        type: post
  ReadinessCheck:
    properties:
      checkInterval:
        description: This is a default description.
        type: post
      healthyThreshold:
        description: This is a default description.
        type: post
      host:
        description: This is a default description.
        type: post
      path:
        description: This is a default description.
        type: post
      timeout:
        description: This is a default description.
        type: post
      unhealthyThreshold:
        description: This is a default description.
        type: post
  RequestUtilization:
    properties:
      targetConcurrentRequests:
        description: This is a default description.
        type: post
      targetRequestCountPerSecond:
        description: This is a default description.
        type: post
  Resources:
    properties:
      cpu:
        description: This is a default description.
        type: post
      diskGb:
        description: This is a default description.
        type: post
      memoryGb:
        description: This is a default description.
        type: post
      volumes:
        description: This is a default description.
        type: post
  ScriptHandler:
    properties:
      scriptPath:
        description: This is a default description.
        type: post
  Service:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  StaticFilesHandler:
    properties:
      applicationReadable:
        description: This is a default description.
        type: post
      expiration:
        description: This is a default description.
        type: post
      httpHeaders:
        description: This is a default description.
        type: post
      mimeType:
        description: This is a default description.
        type: post
      path:
        description: This is a default description.
        type: post
      requireMatchingFile:
        description: This is a default description.
        type: post
      uploadPathRegex:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  TrafficSplit:
    properties:
      allocations:
        description: This is a default description.
        type: post
      shardBy:
        description: This is a default description.
        type: post
  UrlDispatchRule:
    properties:
      domain:
        description: This is a default description.
        type: post
      path:
        description: This is a default description.
        type: post
      service:
        description: This is a default description.
        type: post
  UrlMap:
    properties:
      authFailAction:
        description: This is a default description.
        type: post
      login:
        description: This is a default description.
        type: post
      redirectHttpResponseCode:
        description: This is a default description.
        type: post
      securityLevel:
        description: This is a default description.
        type: post
      urlRegex:
        description: This is a default description.
        type: post
  Version:
    properties:
      betaSettings:
        description: This is a default description.
        type: post
      createTime:
        description: This is a default description.
        type: post
      createdBy:
        description: This is a default description.
        type: post
      defaultExpiration:
        description: This is a default description.
        type: post
      diskUsageBytes:
        description: This is a default description.
        type: post
      env:
        description: This is a default description.
        type: post
      envVariables:
        description: This is a default description.
        type: post
      errorHandlers:
        description: This is a default description.
        type: post
      handlers:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
  Volume:
    properties:
      name:
        description: This is a default description.
        type: post
      sizeGb:
        description: This is a default description.
        type: post
      volumeType:
        description: This is a default description.
        type: post
  ZipInfo:
    properties:
      filesCount:
        description: This is a default description.
        type: post
      sourceUrl:
        description: This is a default description.
        type: post
x-collection-name: Google App Engine
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