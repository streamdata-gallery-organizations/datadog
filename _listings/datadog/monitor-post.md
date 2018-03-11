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
  /monitor:
    post:
      summary: Add Monitor
      description: Create a monitor
      operationId: postMonitor
      parameters:
      - in: query
        name: '#'
        description: |2-
           an integer or decimal number used to set the
                        threshold
        type: string
      - in: query
        name: change_aggr
        description: ' change, pct_change'
        type: string
      - in: query
        name: check
        description: ' name of the check, e'
        type: string
      - in: query
        name: count
        description: |2-
           must be at &gt;= your max threshold (defined
                        in the options)
        type: string
      - in: query
        name: escalation_message
        description: |2-
           a message to include with a
                        re-notification
        type: string
      - in: query
        name: event
        description: ", the event query string:\n                \n                  \nstring_query
          free text query to match against event title and text"
        type: string
      - in: query
        name: event alert
        type: string
      - in: query
        name: excluded_tags
        description: ' exluded event tags (comma-separated)'
        type: string
      - in: query
        name: host
        description: ' event reporting host (comma-separated)'
        type: string
      - in: query
        name: include_tags
        description: |2-
           a boolean indicating whether
                        notifications from this monitor will automatically insert its
                        triggering tags into the title
        type: string
      - in: query
        name: key
        description: |2-
           a 'key' in key:value tag syntax; defines a
                        separate alert for each tag in the group (multi-alert)
        type: string
      - in: query
        name: last
        description: ' the timeframe to roll up the counts'
        type: string
      - in: query
        name: locked
        description: |2-
           a boolean indicating whether changes to
                        to this monitor should be restricted to the creator or admins
        type: string
      - in: query
        name: metric alert
        type: string
      - in: query
        name: notify_audit
        description: |2-
           a boolean indicating whether tagged
                        users will be notified on changes to this monitor
        type: string
      - in: query
        name: notify_no_data
        description: |2-
           a boolean indicating whether this
                        monitor will notify when data stops reporting
        type: string
      - in: query
        name: no_data_timeframe
        description: |2-
           the number of minutes before a
                        monitor will notify when data stops reporting
        type: string
      - in: query
        name: operator
        description: ' &lt;, &lt;=, &gt;, &gt;=, ==, or !='
        type: string
      - in: query
        name: priority
        description: ' event priorities (comma-separated)'
        type: string
      - in: query
        name: renotify_interval
        description: |2-
           the number of minutes after
                        the last notification before a monitor will re-notify on the
                        current status
        type: string
      - in: query
        name: require_full_window
        description: |2-
           a boolean indicating whether
                        this monitor needs a full window of data before it's evaluated
        type: string
      - in: query
        name: role:db
        description: |2
           for a short time:
                                {'role:db': 1412798116}
        type: string
      - in: query
        name: rollup
        description: ' the stats rollup method'
        type: string
      - in: query
        name: service check
        type: string
      - in: query
        name: silenced
        description: |2-
           dictionary of scopes to timestamps or
                        None
        type: string
      - in: query
        name: sources
        description: ' event sources (comma-separated)'
        type: string
      - in: query
        name: space_aggr
        description: ' avg, sum, min, or max'
        type: string
      - in: query
        name: status
        description: ' event statuses (comma-separated)'
        type: string
      - in: query
        name: tags
        description: ' one or more tags (comma-separated), or *'
        type: string
      - in: query
        name: thresholds
        description: |2-
           a dictionary of thresholds by threshold
                        type
        type: string
      - in: query
        name: timeout_h
        description: |2-
           the number of hours of the monitor not
                        reporting data before it will automatically resolve from a
                        triggered state
        type: string
      - in: query
        name: timeshift
        description: |2-
           #m_ago (5, 10, 15, or 30),
                        #h_ago (1, 2, or 4), or 1d_ago
        type: string
      - in: query
        name: time_aggr
        description: ' avg, sum, max, min'
        type: string
      - in: query
        name: 'time_aggr(time_window):space_aggr:metric{tags} [by {key}] operator
          #'
        description: "\n            \n              \ntime_aggr avg, sum, max, min,
          change, or pct_change"
        type: string
      - in: query
        name: time_window
        description: |2-
           last_#m (5, 10, 15, or 30),
                        last_#h (1, 2, or 4), or last_1d
        type: string
      - in: query
        name: '[Triggered] Monitor Title'
        description: |2+

        type: string
      responses:
        200:
          description: OK
      tags:
      - monitoring
      - monitor
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