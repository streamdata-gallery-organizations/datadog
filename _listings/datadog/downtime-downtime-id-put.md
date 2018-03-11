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
  /downtime/:downtime_id:
    put:
      summary: Put Downtime Downtime
      description: Update monitor downtime
      operationId: putDowntimeDowntime
      parameters:
      - in: query
        name: period
        description: ' how often to repeat as an integer'
        type: string
      - in: query
        name: type
        description: ' the type of recurrence'
        type: string
      - in: query
        name: until_date
        description: ' (optional) the date at which the recurrence should end as a
          POSIX timestmap'
        type: string
      - in: query
        name: until_occurrences
        description: ' (optional) how many times the downtime will be rescheduled'
        type: string
      - in: query
        name: week_days
        description: ' (optional) a list of week days to repeat on'
        type: string
      responses:
        200:
          description: OK
      tags:
      - monitoring
      - downtime
      - downtime
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