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
    get:
      summary: ""
      description: List processes for an app
      operationId: apps.app.ps.get
      parameters:
      - in: header
        name: Accept
        description: Content type
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