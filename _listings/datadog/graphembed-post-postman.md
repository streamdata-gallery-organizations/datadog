{
  "info": {
    "name": "DataDog API Add Graph Embed",
    "_postman_id": "f5406b86-2c7b-48bb-bc25-112d0140f63d",
    "description": "Creates a new embeddable graph.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "4dd4fb0d-aa87-4a8a-abcd-dc0e82ca022c",
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
              "id": "5d9e4b91-8a94-4036-937d-73f624ddc1a8"
            }
          ]
        },
        {
          "id": "c2d4b8af-0764-419b-baf5-c1cd4721f647",
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
              "id": "bb765080-a33f-474b-a8c5-7bfa7574ec36"
            }
          ]
        },
        {
          "id": "87103433-e1c1-4b5e-94d4-8f57466038ff",
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
              "id": "427b838a-1096-40d6-b453-9d50e4dacfe3"
            }
          ]
        },
        {
          "id": "6ef6676d-4578-4e6b-967a-308d923c7c34",
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
              "id": "8edc8afa-74ed-4b3c-a617-052c513988a2"
            }
          ]
        },
        {
          "id": "dcbb5603-5fbe-44dd-a403-4a11411b8f95",
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
              "id": "d5737997-557c-4764-9d27-f105a7b2706e"
            }
          ]
        },
        {
          "id": "6848b3cc-3ecb-4559-a6a5-4211e84c01ec",
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
              "id": "539b7629-bcd6-40f4-9c6a-f955bdfd6219"
            }
          ]
        },
        {
          "id": "d6e276d6-12d1-44f8-a121-85ccc3dbe5df",
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
              "id": "8cebdc65-f0d3-425f-983d-0a33e572d906"
            }
          ]
        },
        {
          "id": "d6dd4950-68c5-490f-940a-ae10a08d2968",
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
              "id": "e9bcab80-f039-40a0-8bc5-69d0b328bed3"
            }
          ]
        },
        {
          "id": "4cd14745-e31c-4504-b98d-0c930311f6e5",
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
              "id": "9c1a3211-5834-420e-a900-ab4bb942137f"
            }
          ]
        },
        {
          "id": "e3832221-64ba-457d-a43b-5c4a3913c730",
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
              "id": "aa939e61-7c1c-4ec7-876b-41d3334667cd"
            }
          ]
        },
        {
          "id": "0abf9cd8-68ba-4762-8fad-7febc4e55286",
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
              "id": "085dcb49-db67-4c95-9b67-4ce947a373fa"
            }
          ]
        },
        {
          "id": "9d7e5ec1-35d9-46fd-8c0e-bf2ece38520f",
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
              "id": "8ab97ce9-8516-494b-9430-2f4e1959fcef"
            }
          ]
        },
        {
          "id": "87172d64-0041-42d0-a43e-ef44d02a6680",
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
              "id": "42ce9ef7-03b4-45f2-a4b9-39400b20178b"
            }
          ]
        },
        {
          "id": "78125571-50f3-4b29-ab47-f2db823ca17a",
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
              "id": "acc1ce5b-856d-41e7-a835-56805f22f713"
            }
          ]
        },
        {
          "id": "187130e1-1901-47c3-8ad2-ca5c7c430668",
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
              "id": "cc766543-3fb4-4a68-a40a-507179e598b1"
            }
          ]
        },
        {
          "id": "194aeded-20a6-41c8-ad2f-42530ce2a380",
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
              "id": "6032101b-e4b9-4e94-8837-faf91b60a739"
            }
          ]
        },
        {
          "id": "b0f71fbb-7ac4-4118-aebf-19dd8c316253",
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
              "id": "a65253f9-96db-4f0b-a4df-1f0ad8f74547"
            }
          ]
        },
        {
          "id": "832df15d-794d-4eaa-a03f-6efab522e93e",
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
              "id": "3ddee816-9abf-4e98-9cb8-0d0e5f8a5ce9"
            }
          ]
        },
        {
          "id": "fac6bb69-9a31-481a-ba94-9106230848f3",
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
              "id": "0f5785fb-4a39-49a2-adbe-6c52ff90e5e7"
            }
          ]
        },
        {
          "id": "474bfc22-dd95-42a2-a72a-ef51414d3d57",
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
              "id": "cab18396-4fe8-4aaa-95f6-37cb7c7d0ddf"
            }
          ]
        },
        {
          "id": "aed6c7d9-52a0-4ba1-b2e5-8391b2e51a35",
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
              "id": "f955ab8e-35ab-419a-a412-953c917f044a"
            }
          ]
        },
        {
          "id": "04bbd4d8-0526-4fd0-9512-a312c6696d57",
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
              "id": "bf369e38-5a97-4dc2-b0fd-14c48f35283c"
            }
          ]
        },
        {
          "id": "5bc05faf-8c90-472a-b093-052b25dda584",
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
              "id": "0f3fe80e-d766-4bf8-81d6-668410ed0593"
            }
          ]
        },
        {
          "id": "60d032c4-8aa1-4844-ab05-23de4239e459",
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
              "id": "ca973d28-4b16-4efc-8c9b-1e56d90854cf"
            }
          ]
        },
        {
          "id": "1eb9bf24-ec3e-47f9-909c-aa9e2f231422",
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
              "id": "a8f64f28-57b4-4bd6-bbf0-18ea044ad659"
            }
          ]
        },
        {
          "id": "b3ac8314-8dbd-4131-95c5-c7a6cdb96187",
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
              "id": "1213b685-f3cb-47c4-a93d-442c80f71e31"
            }
          ]
        },
        {
          "id": "f59d6c5a-fbbd-48d3-af88-467ee52d7285",
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
              "id": "a340245e-1ef1-4560-8f11-463b85073fe1"
            }
          ]
        },
        {
          "id": "607fe87a-85e2-4673-b403-2a3d00f9b3ac",
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
              "id": "9c614957-f237-44e2-ac50-523e67574e22"
            }
          ]
        },
        {
          "id": "05b2d38d-902b-4e52-b6c6-ee7c5e3348ab",
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
              "id": "fc2c4592-90d5-40b3-b116-630439c9ea8c"
            }
          ]
        },
        {
          "id": "74999e16-dad0-4fa6-b992-f52d7f045b96",
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
              "id": "861a2332-7e37-40c8-bda6-190516430002"
            }
          ]
        },
        {
          "id": "09567b45-1f54-4370-9c77-2dac14c5ffa8",
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
              "id": "d0927de8-4d33-4d76-8020-89d36457503e"
            }
          ]
        },
        {
          "id": "ea068b0a-292e-4aa2-83b5-095f56c7ad20",
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
              "id": "177de591-557b-4bce-9e8b-a3532032315b"
            }
          ]
        },
        {
          "id": "503ee4f2-18d7-43f6-81d7-2fc8a03622e5",
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
              "id": "e85d0c76-b180-4efd-bea0-fce7d2c00517"
            }
          ]
        },
        {
          "id": "dcd5793d-f893-4e33-829c-6d5e1884a72a",
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
              "id": "eb1cd2d9-a3af-48e4-aa5a-b9033184a9ca"
            }
          ]
        },
        {
          "id": "9e0611d9-ad61-4792-b4d2-3aea938a31a5",
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
              "id": "993eb8f9-2d2e-49f8-8330-0e58e41a0f18"
            }
          ]
        },
        {
          "id": "31c09547-feb1-4d54-944a-39b5db3a5079",
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
              "id": "5efaaea4-602f-4fe9-939c-584afc6186cd"
            }
          ]
        },
        {
          "id": "8f119379-818c-4906-89a4-0e6eb6d18eb3",
          "name": "getDash",
          "request": {
            "url": "http://example.com/api/v1/dash",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all Timeboards"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7939daec-f894-4130-8bf9-50eee6a5aadc"
            }
          ]
        },
        {
          "id": "9c8d6f0f-4e63-4c7e-84ca-d9a29d6e2427",
          "name": "postDash",
          "request": {
            "url": "http://example.com/api/v1/dash?{requests: [{q: system.cpu.idle{} by {host}}=%7Brequests%3A%20%5B%7Bq%3A%20system.cpu.idle%7B%7D%20by%20%7Bhost%7D%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a Timeboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d523ab2b-2d15-4ab2-ac47-d3a99a08fed5"
            }
          ]
        },
        {
          "id": "26b2813a-eacb-4b13-bf97-ca4927f199fb",
          "name": "putDashDash",
          "request": {
            "url": "http://example.com/api/v1/dash/:dash_id?{requests: [{q: system.cpu.idle{} by {host}}=%7Brequests%3A%20%5B%7Bq%3A%20system.cpu.idle%7B%7D%20by%20%7Bhost%7D%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a Timeboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04bfd0e7-ec93-4019-a4d1-b1443d78cc69"
            }
          ]
        },
        {
          "id": "464182b1-cd19-4e87-9de0-4a0df8bf524d",
          "name": "deleteDashDash",
          "request": {
            "url": "http://example.com/api/v1/dash/:dash_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a Timeboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c422720b-70ca-4771-a028-dc96cce28b70"
            }
          ]
        },
        {
          "id": "6c270307-cc06-43ce-b23b-2964277cfd45",
          "name": "getUser",
          "request": {
            "url": "http://example.com/api/v1/user",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "287c9948-5074-4bce-bb87-2b5f135154fb"
            }
          ]
        },
        {
          "id": "3209a3e8-1b82-4d8b-ac33-71775ef91c9e",
          "name": "postUser",
          "request": {
            "url": "http://example.com/api/v1/user",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "POST user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c0500db-e9b6-4f7f-98ad-f00fd75593a8"
            }
          ]
        },
        {
          "id": "20b43cdb-4149-45a8-9a8b-cb2666dcfb0e",
          "name": "getUserHandle",
          "request": {
            "url": "http://example.com/api/v1/user/:handle",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET user handle"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "674d1b88-78e4-40d0-9116-4cb3c6bf157d"
            }
          ]
        },
        {
          "id": "2de2034a-4f2b-4a4a-a3b7-b3dd89c203c8",
          "name": "putUserHandle",
          "request": {
            "url": "http://example.com/api/v1/user/:handle",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Can only be used with application keys belonging to administrators."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "914dfb59-1255-4fb9-90bb-23205e8e5a7d"
            }
          ]
        },
        {
          "id": "c604d5d3-a7a7-480a-938d-0a2ecb02f395",
          "name": "getGraphEmbed",
          "request": {
            "url": "http://example.com/api/v1/graph/embed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of previously created embeddable graphs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4e4eae8-a19a-4e8d-bba4-7c675d54c152"
            }
          ]
        },
        {
          "id": "471d7f30-c97d-4d3f-850f-f4928fbd3129",
          "name": "postGraphEmbed",
          "request": {
            "url": "http://example.com/api/v1/graph/embed",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new embeddable graph."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ba23c24-1776-4816-8b8a-1e5a240c56b0"
            }
          ]
        }
      ]
    }
  ]
}