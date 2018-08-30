{
  "info": {
    "name": "DataDog API Add User",
    "_postman_id": "e93c08d2-69b8-4866-aefd-480c09c1ea81",
    "description": "POST user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "c0f195c2-12a6-49e0-9db7-eab46f512db0",
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
              "id": "a287b635-67ca-410a-9777-cf15817ded0b"
            }
          ]
        },
        {
          "id": "378f5c2a-287a-440e-a0ac-e3f27d2414dc",
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
              "id": "62f5370f-7df0-4450-9d91-bd1be490af1c"
            }
          ]
        },
        {
          "id": "14b88587-64a9-4d9b-8a48-438e8d03a9a4",
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
              "id": "3f045158-29f1-46c2-a493-35d58ba4e83a"
            }
          ]
        },
        {
          "id": "f2d59e05-1e27-433b-ae67-fabbf24e5bb7",
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
              "id": "fb85b338-75fd-4591-b3ed-b82edee64f7e"
            }
          ]
        },
        {
          "id": "78174e41-da2b-47cb-872e-3f1cf40b7c92",
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
              "id": "600eeb63-f399-46f6-9924-36d6780e1554"
            }
          ]
        },
        {
          "id": "5cf83252-52b9-46dd-bd31-ea2d5c4150b3",
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
              "id": "77b4e6dd-3a46-4d09-b391-76ee147cfa68"
            }
          ]
        },
        {
          "id": "5804d583-e718-4d2c-9eea-a0f2f9aec986",
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
              "id": "33e24ab3-fa0b-4e8d-a7ab-23223f9768ba"
            }
          ]
        },
        {
          "id": "a416d67c-d7d0-485e-a49f-2ef313aa62c8",
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
              "id": "b766f801-46f0-4eb5-9fcf-8a766bcb5c3a"
            }
          ]
        },
        {
          "id": "c08d6365-2ea2-4fbd-9b15-14a019b395ed",
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
              "id": "5bfbdeb5-00e5-4494-aeaf-76cfb282662d"
            }
          ]
        },
        {
          "id": "07ebffa5-cfe0-4b7d-9aea-e745e72dc0e7",
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
              "id": "e9a60c8d-87ee-45cc-9bf3-f52967eeb71f"
            }
          ]
        },
        {
          "id": "95d0f6d5-371e-488c-b497-86f8a8ff0555",
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
              "id": "e6ed81fb-4450-4aad-beb6-89fc1fa07db5"
            }
          ]
        },
        {
          "id": "78d5bacb-07f6-48db-8b5f-6e510ba6183d",
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
              "id": "1e911e9f-16db-4290-a564-698de3d2bb40"
            }
          ]
        },
        {
          "id": "7845a51b-508d-4a6a-b4ab-2b4fead03328",
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
              "id": "b626c229-eeaf-453f-bb76-5593a0b4ce13"
            }
          ]
        },
        {
          "id": "a696036f-6fce-4cdf-8620-3ad1a044a6df",
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
              "id": "5226537b-f543-409d-b14f-2c7db46c768b"
            }
          ]
        },
        {
          "id": "63dd80af-52dc-4cbc-9b17-ba1172fd314a",
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
              "id": "38481abd-2516-40a1-bdd8-181c511e1f25"
            }
          ]
        },
        {
          "id": "f60cf35b-b763-4a84-b392-9998a9a2b04a",
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
              "id": "9b689e3d-a0ee-4574-a818-5f71055ad823"
            }
          ]
        },
        {
          "id": "9515ab4e-ff76-49b1-b48a-2aa1a3e93175",
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
              "id": "f19b1121-6915-4193-9b4e-b9f1ded8c1b2"
            }
          ]
        },
        {
          "id": "ab502dc5-aeb8-4172-94b3-f9485901c014",
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
              "id": "6522cc2d-a530-46d9-b532-131e325c7b01"
            }
          ]
        },
        {
          "id": "8bca4324-3304-4df0-aee2-a5a20adba45b",
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
              "id": "143759f4-8e15-4028-b95a-29c697ec7713"
            }
          ]
        },
        {
          "id": "25d2cb93-3b63-4479-ad66-65aa6112d07b",
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
              "id": "0022756c-fe01-4704-9d39-3d4e4dcd90b6"
            }
          ]
        },
        {
          "id": "56c3bc33-514a-4e7a-ba42-9570c2172fad",
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
              "id": "507b6702-a752-4866-94d7-b9be0a9b849a"
            }
          ]
        },
        {
          "id": "ba1ece57-178b-4fa3-bf63-b1c2da6ee004",
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
              "id": "a924d0c5-ac52-4e63-8db3-0c4383ed9323"
            }
          ]
        },
        {
          "id": "814bc2d4-7fca-494e-a5b5-5c6b91d4fa0f",
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
              "id": "631a08a2-5b10-498a-81aa-a15462d054d0"
            }
          ]
        },
        {
          "id": "c7cd0cba-6bac-4f41-affc-3c3f66004814",
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
              "id": "6c57681b-8537-4072-9ce3-03359c2e4a95"
            }
          ]
        },
        {
          "id": "c8187183-d707-4cc1-bab8-b9277f2da9ae",
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
              "id": "44359f92-c74c-45dc-b5f9-ac49e0adabb3"
            }
          ]
        },
        {
          "id": "70454667-191c-4866-80d7-45edbab60a06",
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
              "id": "470f78ab-0291-4e05-bd91-17ba8b1bee6e"
            }
          ]
        },
        {
          "id": "c05c560c-e9c6-4347-beab-010a301c8697",
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
              "id": "76c25b5f-09b2-45b1-a1e9-39e18422308a"
            }
          ]
        },
        {
          "id": "a0a7d50a-8508-4e32-bc84-24027c434e24",
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
              "id": "bffcce30-3b97-4a16-a339-1f43baeb7b08"
            }
          ]
        },
        {
          "id": "0e8114f2-4400-46d5-9df6-0b18178cb8ec",
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
              "id": "df21ad74-351c-491b-a814-be285f2e71fb"
            }
          ]
        },
        {
          "id": "f1d6c928-7be1-40ab-8e35-7903ecbc0bd9",
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
              "id": "4b504e27-c54d-45fa-8d4f-2fe2ed42373a"
            }
          ]
        },
        {
          "id": "108aae2b-1593-48c8-bab4-ef47e2fbfa53",
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
              "id": "ada85496-724f-481f-8a80-685a772c4d6c"
            }
          ]
        },
        {
          "id": "8c5a69ca-6d10-4ad9-9695-d13ef5fc7239",
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
              "id": "68577ecc-ac77-413f-92c6-a1243d530315"
            }
          ]
        },
        {
          "id": "b050d218-171b-4872-9295-3f0ebf2670ba",
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
              "id": "34f91a99-fbca-4e17-b401-fb7f8f004d6f"
            }
          ]
        },
        {
          "id": "050689bf-d908-4366-867c-ab67d891f558",
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
              "id": "271bb4d0-73c6-4463-841a-9c6fda8a7488"
            }
          ]
        },
        {
          "id": "209db49f-3b2b-4889-8a60-c37e2f02eda6",
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
              "id": "811264d2-7d5e-4991-bfee-36ecf16ca212"
            }
          ]
        },
        {
          "id": "a3cb2925-f770-426c-ad39-430c5cf8b417",
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
              "id": "d461972b-cd75-4220-81f4-acf386f490e6"
            }
          ]
        },
        {
          "id": "1f53c8c0-d5a5-46b3-bb18-37116c49aee1",
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
              "id": "f4359ed5-cdbd-4d1a-903b-55d4cb751f06"
            }
          ]
        },
        {
          "id": "b8a22eb6-576f-4d1e-96ec-f4523c311f2e",
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
              "id": "ad609188-f7c3-4ef4-b391-cded58313002"
            }
          ]
        },
        {
          "id": "0d074b09-0eab-4969-b7a2-7d246d93dea8",
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
              "id": "efe04eb9-750a-4e85-84ae-c87c1fdfe7e1"
            }
          ]
        },
        {
          "id": "b729e50a-ea40-494c-91a3-f624a97ff8c2",
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
              "id": "a006f2d8-9ce2-4768-965d-fd8f6a35c3d3"
            }
          ]
        },
        {
          "id": "2286b42b-3a57-4f31-9b49-52ba5246cbf0",
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
              "id": "44885058-14f4-4c6d-973f-2a7606c2a6a0"
            }
          ]
        }
      ]
    }
  ]
}