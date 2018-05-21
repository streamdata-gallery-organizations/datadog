{
  "info": {
    "name": "DataDog API Add Monitor Monitor  Mute",
    "_postman_id": "5826975f-fd4a-4084-aa4e-87159c50fdf1",
    "description": "POST monitor monitor  mute",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "3b22adda-8f76-4619-93f6-f6d528e4d317",
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
              "id": "fbab4dc5-caae-4262-88d3-6d0440cc7635"
            }
          ]
        },
        {
          "id": "74ebbddf-a162-4213-9258-5af0b527ad4c",
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
              "id": "03020867-e98c-42e9-a787-244e1fcebb10"
            }
          ]
        },
        {
          "id": "1aec6b7e-1e4a-4b4a-9128-148390f9efcd",
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
              "id": "f23b472f-e4f5-4c3d-912b-6021d25542a9"
            }
          ]
        },
        {
          "id": "94027a20-ecbb-47cc-9bab-aba82215af6f",
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
              "id": "39f21384-4553-4353-9b46-ed3db6385670"
            }
          ]
        },
        {
          "id": "10da01b9-74e6-4f4f-88e4-402d57728c82",
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
              "id": "66860f20-709a-4aed-bb45-f8779b52dc05"
            }
          ]
        },
        {
          "id": "c0043650-1f3e-4724-b49c-7281b852070c",
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
              "id": "7eddbdf1-75fe-4c23-8d2b-543ac10b6f16"
            }
          ]
        },
        {
          "id": "86af8b5d-a367-4d68-aead-f44550ba7ee1",
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
              "id": "19b4c6c0-a4a0-4823-b587-f1328889ac22"
            }
          ]
        },
        {
          "id": "ce8f45cb-4cc8-4a82-b02d-e1c1f3a16a2f",
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
              "id": "85e2af1a-82e4-4f03-8e93-eb2ac8562348"
            }
          ]
        },
        {
          "id": "123e0eb4-8220-41ee-aabb-3c1fe1af5e29",
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
              "id": "c3baa478-c425-40a7-8883-ea04a5818211"
            }
          ]
        },
        {
          "id": "98ca6f9d-d34d-4d7b-931a-f312c870d592",
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
              "id": "b3e04c9b-5922-42bf-947b-809b9c40a3b9"
            }
          ]
        },
        {
          "id": "62a65d30-6c08-416e-a584-517415f62bc2",
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
              "id": "f0c9b666-e038-4432-8d8f-824629ddbfd1"
            }
          ]
        },
        {
          "id": "d8345abf-56b4-4a6c-b4a6-4a06dfbc87ca",
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
              "id": "ae7b676e-1bfb-44db-a2a4-d027101541fc"
            }
          ]
        },
        {
          "id": "1bf8bbff-41c2-4555-bea0-b7c59313fd6e",
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
              "id": "5e291738-c9e2-43ee-887f-3c0343e4df64"
            }
          ]
        },
        {
          "id": "25897240-76c1-45ca-b374-c94ddc882b76",
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
              "id": "116534c1-5404-4529-959b-efadeb3bc695"
            }
          ]
        },
        {
          "id": "945dfae6-eec6-49d1-8147-69f3d12cfe0a",
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
              "id": "b7efec76-fa4e-4932-9190-7412b68572be"
            }
          ]
        },
        {
          "id": "069dc4c3-7171-4106-b2f0-8580a5444d19",
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
              "id": "887cecae-f219-488e-bda2-2ac6c713a914"
            }
          ]
        },
        {
          "id": "43abdfc8-9ed4-4ed6-9379-da32411865d1",
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
              "id": "65c39691-12c4-44ca-8679-543296fe1802"
            }
          ]
        },
        {
          "id": "ed9a63c0-cdae-447c-af2d-6e9d18f3608a",
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
              "id": "11a24266-3ec4-4f29-b00c-e2b6c3b4b297"
            }
          ]
        },
        {
          "id": "e40b3b4f-9f53-4896-902f-100f6a07af5f",
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
              "id": "88b68938-224f-4766-9b8b-f8a44059b83f"
            }
          ]
        },
        {
          "id": "dc377e3e-6f5c-4f9d-8153-0ba67de99c61",
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
              "id": "089eb5d4-52dd-4b6b-a1eb-ba58785bc966"
            }
          ]
        },
        {
          "id": "c98e1edd-8b02-40a8-b0f9-8dc075e32de6",
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
              "id": "0add1a52-680a-4df3-aaca-6ef2faa05c20"
            }
          ]
        },
        {
          "id": "4bdab6cf-2bec-4041-b410-6e9be4afcefc",
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
              "id": "21e7da27-1b22-4e55-8503-ebc30780c619"
            }
          ]
        },
        {
          "id": "e02869ca-4b6f-432b-b1f2-3f0f1a89ffe1",
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
              "id": "2b878d54-70b2-4f5b-89ee-855e1ff33a70"
            }
          ]
        },
        {
          "id": "459e196e-178c-46ad-a0ec-a8b40d75786d",
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
              "id": "2f5d53eb-3675-49af-86fe-6687d17bbdca"
            }
          ]
        },
        {
          "id": "55f6f458-76c5-4433-91d6-cb4e555d582e",
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
              "id": "dc5b15be-3a53-497e-8f85-62d7ae50359a"
            }
          ]
        },
        {
          "id": "cff4d65b-bb76-4cc5-999c-c0b86ee7fa59",
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
              "id": "4d9709c5-654c-4135-aeba-17419b11f9a6"
            }
          ]
        },
        {
          "id": "b0a83626-a5cc-4bcb-a73c-45192a3e6187",
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
              "id": "3087eab6-9f42-4a9f-960a-60c2173be6f9"
            }
          ]
        },
        {
          "id": "c5d447b9-4e7f-4908-88ed-fe8ffbfefda8",
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
              "id": "ed7612ad-ee49-471f-ba28-007483a0b9f2"
            }
          ]
        },
        {
          "id": "8fa951b0-bd35-4dfe-af1f-798f8667cefb",
          "name": "getMonitor",
          "request": {
            "url": "http://example.com/api/v1/monitor",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all monitor details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78cd4b0a-ebdc-4925-ac49-d6789c6b382a"
            }
          ]
        },
        {
          "id": "b15e77fc-a80c-4309-bb65-73fd50da383f",
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
              "id": "0a4567d4-da86-4f4c-a780-e53cee0e5069"
            }
          ]
        },
        {
          "id": "c0f25149-69bd-40c0-949b-60baa46c93c5",
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
              "id": "d5f18175-2640-4785-ac4a-c26641e0e882"
            }
          ]
        },
        {
          "id": "3124b2ca-007e-49cc-aad3-d9087a949db0",
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
              "id": "54237a4d-78d3-4b67-be1c-af122e7e54d0"
            }
          ]
        },
        {
          "id": "3888e1e3-7c7c-4529-a4a2-7cbda134e116",
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
              "id": "4c4e05e7-ac56-4f09-bfcc-c2899ac01b54"
            }
          ]
        },
        {
          "id": "9d9e829c-828a-4837-ba60-0924c5a734f6",
          "name": "postMonitorMuteAll",
          "request": {
            "url": "http://example.com/api/v1/monitor/mute_all",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Muting will prevent all monitors from notifying through email and posts\n        to the event stream. State changes will only be visible by checking\n        the alert page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffd0a5ea-16a8-4194-9e2c-a0f26316627a"
            }
          ]
        },
        {
          "id": "54a9595c-1a7c-4341-83ab-d81868af5c5b",
          "name": "postMonitorUnmuteAll",
          "request": {
            "url": "http://example.com/api/v1/monitor/unmute_all",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Disables muting all monitors. Throws an error if mute all was\n        not enabled previously."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccf94bfa-77a6-4ec9-b370-1ffe4517f3d7"
            }
          ]
        },
        {
          "id": "f59554bf-99e5-447a-8034-973c06da8adb",
          "name": "postMonitorMonitorMute",
          "request": {
            "url": "http://example.com/api/v1/monitor/:monitor_id/mute",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "POST monitor monitor  mute"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0177c41e-fe46-430a-a3d1-c7b12eddf2d5"
            }
          ]
        }
      ]
    }
  ]
}