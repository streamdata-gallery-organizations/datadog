---
swagger: "2.0"
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dash/:dash_id:
    put:
      summary: Put Dash Dash
      description: Update a Timeboard
      operationId: putDashDash
      parameters:
      - in: query
        name: '{requests: [{q: system.cpu.idle{*} by {host}}'
        description: "\n                \n              \n            "
        type: string
      responses:
        200:
          description: OK
      tags:
      - monitoring
      - dash
      - dash
definitions: []
x-collection-name: DataDog
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