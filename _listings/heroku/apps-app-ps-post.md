---
swagger: "2.0"
info:
  title: Heroku
  description: Manage your Heroku apps, configs, collaborators &amp; resources
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/{app}/ps:
    post:
      summary: ""
      description: Run a one-off process
      operationId: apps.app.ps.post
      parameters:
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: attach
        description: 'true: use rendezvous to access stdin/stdout - <blank>: stream
          process output to the application log'
      - in: query
        name: command
        description: The command to run
      responses:
        200:
          description: OK
      tags:
      - ""
definitions: []
x-collection-name: Heroku
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