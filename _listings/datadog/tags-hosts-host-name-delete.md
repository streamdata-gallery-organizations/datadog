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
  /tags/hosts/:host_name:
    delete:
      summary: Delete Tags Hosts Host Name
      description: |2-

                  This end point allows you to remove all tags for a given host
      operationId: deleteTagsHostsHostName
      responses:
        200:
          description: OK
      tags:
      - monitoring
      - tags
      - hosts
      - host
      - name
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