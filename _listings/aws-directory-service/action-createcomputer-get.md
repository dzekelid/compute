---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateComputer:
    get:
      summary: ' Create Computer '
      description: Creates a computer account in the specified directory, and joins
        the computer to the directory
      operationId: createComputer
      parameters:
      - in: query
        name: ComputerAttributes
        description: An array of Attribute objects that contain any LDAP attributes
          to apply to the            computer account
        type: string
      - in: query
        name: ComputerName
        description: The name of the computer account
        type: string
      - in: query
        name: DirectoryId
        description: The identifier of the directory in which to create the computer
          account
        type: string
      - in: query
        name: OrganizationalUnitDistinguishedName
        description: The fully-qualified distinguished name of the organizational
          unit to place the computer account in
        type: string
      - in: query
        name: Password
        description: A one-time password that is used to join the computer to the
          directory
        type: string
      responses:
        200:
          description: OK
      tags:
      - computer
definitions: []
x-collection-name: AWS Directory Service
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