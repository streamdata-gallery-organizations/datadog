{
  "info": {
    "name": "DataDog API Delete Monitor Monitor",
    "_postman_id": "3cc43182-6507-4c0b-877b-a843bce55e78",
    "description": "DELETE monitor monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "b400745d-f3e8-44dc-901f-37d5cafa5a57",
          "name": "getMetrics",
          "request": {
            "url": "http://example.com/api/v1/metrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of actively reporting metrics from a given time until now. This endpoint is not available in the Python and Ruby libraries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "136c3585-1743-4751-99df-1f06be057da8"
            }
          ]
        },
        {
          "id": "5f7cf70f-a829-4104-994b-ff8a56fa8804",
          "name": "postSeries",
          "request": {
            "url": "http://example.com/api/v1/series?[[POSIX_timestamp, numeric_value], ...]=%5B%5BPOSIX_timestamp%2C%20numeric_value%5D%2C%20...%5D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The metrics end-point allows you to post time-series data that can be\n          graphed on Datadog's dashboards."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "918bde6c-3ee3-4ac1-8725-b09140fd1bc1"
            }
          ]
        },
        {
          "id": "338b7a32-12a4-4727-bfba-681cff463135",
          "name": "getQuery",
          "request": {
            "url": "http://example.com/api/v1/query",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to query for metrics from any time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "504d8d5b-79ba-44b2-a815-79439cbb8630"
            }
          ]
        },
        {
          "id": "c6c7bb6f-6b39-4370-ac13-440915a63a67",
          "name": "postCheckRun",
          "request": {
            "url": "http://example.com/api/v1/check_run",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post a Check Run"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "536d1816-ea62-4456-8cf2-03d236e4bfc7"
            }
          ]
        },
        {
          "id": "ac8289ee-ae64-469b-b646-2c15a353620a",
          "name": "getDowntime",
          "request": {
            "url": "http://example.com/api/v1/downtime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all monitor downtimes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6485dfb9-359c-46f0-9c47-cdce42f45738"
            }
          ]
        },
        {
          "id": "7e478b88-b490-4376-8fbc-4b529e84ca1d",
          "name": "postDowntime",
          "request": {
            "url": "http://example.com/api/v1/downtime?period=period&type=type&until_date=until_date&until_occurrences=until_occurrences&week_days=week_days",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Schedule monitor downtime"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a310177-64b0-4aeb-9f0e-26fc6437c83d"
            }
          ]
        },
        {
          "id": "1f8b01e1-5125-45ed-a1f1-2084adb1fbac",
          "name": "getDowntimeDowntime",
          "request": {
            "url": "http://example.com/api/v1/downtime/:downtime_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a monitor downtime"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ac3890d-9811-43ff-b1c9-d56a9595b4a6"
            }
          ]
        },
        {
          "id": "7d3be0cc-6c52-4466-b185-92fb7df4d8b6",
          "name": "putDowntimeDowntime",
          "request": {
            "url": "http://example.com/api/v1/downtime/:downtime_id?period=period&type=type&until_date=until_date&until_occurrences=until_occurrences&week_days=week_days",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update monitor downtime"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a84b5aa-48db-49af-9110-f92419e75a30"
            }
          ]
        },
        {
          "id": "58e7b154-9baf-4d13-90c9-c4bbc6a25ef3",
          "name": "deleteDowntimeDowntime",
          "request": {
            "url": "http://example.com/api/v1/downtime/:downtime_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DELETE downtime downtime"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f47f314-64a0-4659-9ff1-f57f06451613"
            }
          ]
        },
        {
          "id": "8ab7612b-3251-43ea-b7dd-7990292cea4f",
          "name": "getScreen",
          "request": {
            "url": "http://example.com/api/v1/screen",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch all of your screenboards' definitions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c47272e0-be9e-4bb0-ae59-d9d36e39d9cb"
            }
          ]
        },
        {
          "id": "af28af77-af86-43b8-9878-f4dce88f5812",
          "name": "postScreen",
          "request": {
            "url": "http://example.com/api/v1/screen",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "POST screen"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ffbf00d-f31b-47f4-b982-754c8825c3b4"
            }
          ]
        },
        {
          "id": "a5600328-4d12-4da1-98b1-904a19fcc30e",
          "name": "getScreenBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/:board_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch an existing screenboard's definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "add5f988-eabb-4142-82a7-b0e49fed0c73"
            }
          ]
        },
        {
          "id": "0b140979-1093-4eab-8542-11f212f8346c",
          "name": "putScreenBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/:board_id",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "PUT screen board"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "272d795e-19d4-4231-958e-fa8b441028b5"
            }
          ]
        },
        {
          "id": "e0af7fef-cc5c-46f7-ac58-02c2f46fa967",
          "name": "deleteScreenBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/:board_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an existing screenboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0178919-3e99-47ef-bc40-768413ce07dc"
            }
          ]
        },
        {
          "id": "23dcb2e7-b14e-40a6-a4aa-4e312ec481f6",
          "name": "getScreenShareBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/share/:board_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Share an existing screenboard's with a public URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42f47e03-c508-4ffb-988a-7b8b89c9e93b"
            }
          ]
        },
        {
          "id": "40a91287-b29c-4c35-8a3a-8c2ef3571df6",
          "name": "deleteScreenShareBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/share/:board_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Revoke a currently shared screenboard's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db67308b-f323-4faf-933f-a8defc5949f6"
            }
          ]
        },
        {
          "id": "877339d3-008c-4951-b100-499b6c79e486",
          "name": "getTagsHosts",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a mapping of tags to hosts for your whole infrastructure."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f567a856-947d-4228-ac87-8822ee07b5b1"
            }
          ]
        },
        {
          "id": "f16110bb-a53d-4a4c-80f4-2a57d64c82ce",
          "name": "getTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of tags that apply to a given host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b509c7a-42c4-4cf7-8970-69158583a1f1"
            }
          ]
        },
        {
          "id": "aabd52c2-eb4b-4e0a-b654-c842051f05cd",
          "name": "putTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to update all tags for a given host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ff6fc22-6e44-489b-a11a-bc1fb9ce7c9a"
            }
          ]
        },
        {
          "id": "f5cc5686-e07e-43c7-ab01-ad8092aa22dc",
          "name": "postTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to add tags to a host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d925daf6-5c99-4c1c-9c0b-e50e4bf2b295"
            }
          ]
        },
        {
          "id": "dc5c7524-7eaf-49c2-a45b-d75ca8057f18",
          "name": "deleteTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to remove all tags for a given host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9eb9ce4-a940-43cd-872f-85237eb9ef7a"
            }
          ]
        },
        {
          "id": "14802d99-a4ac-46a9-9978-b644d838691f",
          "name": "postComments",
          "request": {
            "url": "http://example.com/api/v1/comments",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Comments are essentially special forms of events that\n          appear in the stream. They can start a new discussion thread or\n          optionally, reply in another thread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b057b761-b6c2-4cd3-aa9c-cb47691f86e5"
            }
          ]
        },
        {
          "id": "8c51428d-49cf-4e3f-8133-7366e5cc171b",
          "name": "putCommentsComment",
          "request": {
            "url": "http://example.com/api/v1/comments/:comment_id",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "PUT comments comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "924621d0-1d1a-44cb-bd40-7bc4bf3e21ce"
            }
          ]
        },
        {
          "id": "d4b0cb00-9aad-4d15-8ded-2d5c77f2acd8",
          "name": "deleteCommentsComment",
          "request": {
            "url": "http://example.com/api/v1/comments/:comment_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DELETE comments comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6d745b0-d577-447c-a431-6622e18acbe8"
            }
          ]
        },
        {
          "id": "a8c99c82-933d-4d32-82ae-82bbb769f4fc",
          "name": "getGraphSnapshot",
          "request": {
            "url": "http://example.com/api/v1/graph/snapshot?graph_def=graph_def",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET graph snapshot"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7f7cc29-59d1-4ae9-bdb3-dd24512d52e4"
            }
          ]
        },
        {
          "id": "28216d77-531e-4653-a594-37f8bdb4a95a",
          "name": "postEvents",
          "request": {
            "url": "http://example.com/api/v1/events",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post an Event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3e098e0-5f77-4943-a522-07a9743a62ca"
            }
          ]
        },
        {
          "id": "4f4b8aca-68f8-449d-b5e8-aae888fb9408",
          "name": "getEventsEvent",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET events event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b3ed35e-23ef-48d8-a2b3-6d9ea32ee91c"
            }
          ]
        },
        {
          "id": "db7a203e-8fad-4db1-92f5-2c85809e0d0d",
          "name": "deleteEventsEvent",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DELETE events event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbd36089-c9ba-47c0-95eb-a0102e16c007"
            }
          ]
        },
        {
          "id": "e55d0eaf-4c5c-4824-a005-a5938b86557b",
          "name": "postMonitor",
          "request": {
            "url": "http://example.com/api/v1/monitor?#=%23&change_aggr=change_aggr&check=check&count=count&escalation_message=escalation_message&event=event&event alert=event%20alert&excluded_tags=excluded_tags&host=host&include_tags=include_tags&key=key&last=last&locked=locked&metric alert=metric%20alert&notify_audit=notify_audit&notify_no_data=notify_no_data&no_data_timeframe=no_data_timeframe&operator=operator&priority=priority&renotify_interval=renotify_interval&require_full_window=require_full_window&role:db=role%3Adb&rollup=rollup&service check=service%20check&silenced=silenced&sources=sources&space_aggr=space_aggr&status=status&tags=tags&thresholds=thresholds&timeout_h=timeout_h&timeshift=timeshift&time_aggr=time_aggr&time_aggr(time_window):space_aggr:metric{tags} [by {key}] operator #=time_aggr%28time_window%29%3Aspace_aggr%3Ametric%7Btags%7D%20%5Bby%20%7Bkey%7D%5D%20operator%20%23&time_window=time_window&[Triggered] Monitor Title=%5BTriggered%5D%20Monitor%20Title",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00823029-0848-4ac3-9162-b4edbf76dd69"
            }
          ]
        },
        {
          "id": "327a2dca-5fc6-45fe-be18-7198a77c00f7",
          "name": "getMonitorMonitor",
          "request": {
            "url": "http://example.com/api/v1/monitor/:monitor_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET monitor monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8de38e21-04ee-4bb9-8b97-fecef945ad9d"
            }
          ]
        },
        {
          "id": "47194374-8044-4429-87ac-a233124ffb26",
          "name": "putMonitorMonitor",
          "request": {
            "url": "http://example.com/api/v1/monitor/:monitor_id",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "PUT monitor monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d5f2d4b-f543-4568-8147-f5f43524fd5e"
            }
          ]
        },
        {
          "id": "fb59ae63-a5c3-407c-b20a-73431aa70890",
          "name": "deleteMonitorMonitor",
          "request": {
            "url": "http://example.com/api/v1/monitor/:monitor_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DELETE monitor monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bba1621-fcd4-431e-b1f0-bd7201dbee15"
            }
          ]
        }
      ]
    }
  ]
}