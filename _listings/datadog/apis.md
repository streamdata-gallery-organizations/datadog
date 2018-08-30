---
name: Datadog
x-slug: datadog
description: See inside any stack, any app, at any scale, anywhere.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
x-kinRank: "8"
x-alexaRank: "13593"
tags: Datadog
created: "2018-08-29"
modified: "2018-08-29"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/apis.md
specificationVersion: "0.14"
apis:
- name: DataDog Merged API - Get Metrics
  x-api-slug: metrics-get
  description: Get the list of actively reporting metrics from a given time until
    now. This endpoint is not available in the Python and Ruby libraries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/metrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/metrics-get-openapi.md
- name: DataDog Merged API - Add Series
  x-api-slug: series-post
  description: |-
    The metrics end-point allows you to post time-series data that can be
              graphed on Datadog's dashboards.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/series-post-openapi.md
- name: DataDog Merged API - Get Query
  x-api-slug: query-get
  description: This end point allows you to query for metrics from any time period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/query-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/query-get-openapi.md
- name: DataDog Merged API - Add Check Run
  x-api-slug: check-run-post
  description: Post a Check Run
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/check-run-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/check-run-post-openapi.md
- name: DataDog Merged API - Add Downtime
  x-api-slug: downtime-post
  description: Schedule monitor downtime
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtime-post-openapi.md
- name: DataDog Merged API - Put Downtime Downtime
  x-api-slug: downtimedowntime-id-put
  description: Update monitor downtime
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtimedowntime-id-put-openapi.md
- name: DataDog Merged API - Delete Downtime Downtime
  x-api-slug: downtimedowntime-id-delete
  description: DELETE downtime downtime
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtimedowntime-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtimedowntime-id-delete-openapi.md
- name: DataDog Merged API - Get Downtime Downtime
  x-api-slug: downtimedowntime-id-get
  description: Get a monitor downtime
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtimedowntime-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtimedowntime-id-get-openapi.md
- name: DataDog Merged API - Get Downtime
  x-api-slug: downtime-get
  description: Get all monitor downtimes
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/downtime-get-openapi.md
- name: DataDog Merged API - Add Screen
  x-api-slug: screen-post
  description: POST screen
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screen-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screen-post-openapi.md
- name: DataDog Merged API - Put Screen Board
  x-api-slug: screenboard-id-put
  description: PUT screen board
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenboard-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenboard-id-put-openapi.md
- name: DataDog Merged API - Delete Screen Board
  x-api-slug: screenboard-id-delete
  description: Delete an existing screenboard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenboard-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenboard-id-delete-openapi.md
- name: DataDog Merged API - Get Screen Board
  x-api-slug: screenboard-id-get
  description: Fetch an existing screenboard's definition.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenboard-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenboard-id-get-openapi.md
- name: DataDog Merged API - Get Screen
  x-api-slug: screen-get
  description: Fetch all of your screenboards' definitions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screen-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screen-get-openapi.md
- name: DataDog Merged API - Get Screen Share Board
  x-api-slug: screenshareboard-id-get
  description: Share an existing screenboard's with a public URL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenshareboard-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenshareboard-id-get-openapi.md
- name: DataDog Merged API - Delete Screen Share Board
  x-api-slug: screenshareboard-id-delete
  description: Revoke a currently shared screenboard's.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenshareboard-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/screenshareboard-id-delete-openapi.md
- name: DataDog Merged API - Get Tags Hosts
  x-api-slug: tagshosts-get
  description: Return a mapping of tags to hosts for your whole infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/tagshosts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/tagshosts-get-openapi.md
- name: DataDog Merged API - Get Tags Hosts Host Name
  x-api-slug: tagshostshost-name-get
  description: Return the list of tags that apply to a given host.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/tagshostshost-name-get-openapi.md
- name: DataDog Merged API - Add Tags Hosts Host Name
  x-api-slug: tagshostshost-name-post
  description: This end point allows you to add tags to a host.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/tagshostshost-name-post-openapi.md
- name: DataDog Merged API - Put Tags Hosts Host Name
  x-api-slug: tagshostshost-name-put
  description: This end point allows you to update all tags for a given host.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/tagshostshost-name-put-openapi.md
- name: DataDog Merged API - Delete Tags Hosts Host Name
  x-api-slug: tagshostshost-name-delete
  description: This end point allows you to remove all tags for a given host.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/tagshostshost-name-delete-openapi.md
- name: DataDog Merged API - Add Comments
  x-api-slug: comments-post
  description: |-
    Comments are essentially special forms of events that
              appear in the stream. They can start a new discussion thread or
              optionally, reply in another thread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/comments-post-openapi.md
- name: DataDog Merged API - Put Comments Comment
  x-api-slug: commentscomment-id-put
  description: PUT comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/commentscomment-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/commentscomment-id-put-openapi.md
- name: DataDog Merged API - Delete Comments Comment
  x-api-slug: commentscomment-id-delete
  description: DELETE comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/commentscomment-id-delete-openapi.md
- name: DataDog Merged API - Get Graph Snapshot
  x-api-slug: graphsnapshot-get
  description: GET graph snapshot
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphsnapshot-get-openapi.md
- name: DataDog Merged API - Add Events
  x-api-slug: events-post
  description: Post an Event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/events-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/events-post-openapi.md
- name: DataDog Merged API - Get Events Event
  x-api-slug: eventsevent-id-get
  description: GET events event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/eventsevent-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/eventsevent-id-get-openapi.md
- name: DataDog Merged API - Delete Events Event
  x-api-slug: eventsevent-id-delete
  description: DELETE events event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/eventsevent-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/eventsevent-id-delete-openapi.md
- name: DataDog Merged API - Add Monitor
  x-api-slug: monitor-post
  description: Create a monitor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitor-post-openapi.md
- name: DataDog Merged API - Get Monitor Monitor
  x-api-slug: monitormonitor-id-get
  description: GET monitor monitor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-id-get-openapi.md
- name: DataDog Merged API - Put Monitor Monitor
  x-api-slug: monitormonitor-id-put
  description: PUT monitor monitor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-id-put-openapi.md
- name: DataDog Merged API - Delete Monitor Monitor
  x-api-slug: monitormonitor-id-delete
  description: DELETE monitor monitor
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-id-delete-openapi.md
- name: DataDog Merged API - Get Monitor
  x-api-slug: monitor-get
  description: Get all monitor details
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitor-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitor-get-openapi.md
- name: DataDog Merged API - Add Monitor Mute All
  x-api-slug: monitormute-all-post
  description: |-
    Muting will prevent all monitors from notifying through email and posts
            to the event stream. State changes will only be visible by checking
            the alert page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormute-all-post-openapi.md
- name: DataDog Merged API - Add Monitor Unmute All
  x-api-slug: monitorunmute-all-post
  description: |-
    Disables muting all monitors. Throws an error if mute all was
            not enabled previously.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitorunmute-all-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitorunmute-all-post-openapi.md
- name: DataDog Merged API - Add Monitor Monitor  Mute
  x-api-slug: monitormonitor-idmute-post
  description: POST monitor monitor  mute
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-idmute-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/monitormonitor-idmute-post-openapi.md
- name: DataDog Merged API - Add Dash
  x-api-slug: dash-post
  description: Create a Timeboard
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/dash-post-openapi.md
- name: DataDog Merged API - Put Dash Dash
  x-api-slug: dashdash-id-put
  description: Update a Timeboard
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/dashdash-id-put-openapi.md
- name: DataDog Merged API - Delete Dash Dash
  x-api-slug: dashdash-id-delete
  description: Delete a Timeboard
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/dashdash-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/dashdash-id-delete-openapi.md
- name: DataDog Merged API - Get Dash
  x-api-slug: dash-get
  description: Get all Timeboards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/dash-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/dash-get-openapi.md
- name: DataDog Merged API - Add User
  x-api-slug: user-post
  description: POST user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/user-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/user-post-openapi.md
- name: DataDog Merged API - Get User Handle
  x-api-slug: userhandle-get
  description: GET user handle
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/userhandle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/userhandle-get-openapi.md
- name: DataDog Merged API - Get User
  x-api-slug: user-get
  description: GET user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/user-get-openapi.md
- name: DataDog Merged API - Put User Handle
  x-api-slug: userhandle-put
  description: Can only be used with application keys belonging to administrators.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/userhandle-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/userhandle-put-openapi.md
- name: DataDog Merged API - Get Graph Embed
  x-api-slug: graphembed-get
  description: Gets a list of previously created embeddable graphs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphembed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphembed-get-openapi.md
- name: DataDog Merged API - Add Graph Embed
  x-api-slug: graphembed-post
  description: Creates a new embeddable graph.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphembed-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphembed-post-openapi.md
- name: DataDog Merged API - Get Graph Embed Embed
  x-api-slug: graphembedembed-id-get
  description: Get the HTML fragment for a previously generated embed with embed_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphembedembed-id-get-openapi.md
- name: DataDog Merged API - Get Graph Embed Embed  Enable
  x-api-slug: graphembedembed-idenable-get
  description: Enable a specified embed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22961-datadog.jpg
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Monitoring, Performance, Orchestration, Aggregation, Stack Network, SaaS,
    Technology, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/datadog/master/_listings/datadog/graphembedembed-idenable-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://dataatwork.api.gallery.streamdata.io
- type: x-api-stack
  url: http://datadog.stack.network
- type: x-blog
  url: https://www.datadoghq.com/blog/
- type: x-blog-rss
  url: https://www.datadoghq.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/datadog
- type: x-email
  url: info@datadoghq.com
- type: x-email
  url: help@datadoghq.com
- type: x-email
  url: legalcompliance@datadoghq.com
- type: x-email
  url: legal@datadoghq.com
- type: x-email
  url: iwant@datadoghq.com
- type: x-github
  url: https://github.com/datadog
- type: x-twitter
  url: https://twitter.com/datadoghq
- type: x-integrations
  url: https://www.datadoghq.com/product/integrations/
- type: x-pricing
  url: https://www.datadoghq.com/pricing/
- type: x-security
  url: https://www.datadoghq.com/security/
- type: x-website
  url: https://www.datadoghq.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---