{
  "info": {
    "name": "DataDog API Get Dash",
    "_postman_id": "ac05326a-5fdf-43b4-8574-afe780c9b569",
    "description": "Get all Timeboards",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "7a97738b-d90a-4978-8ba6-846d13050097",
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
              "id": "6efbb4f1-77de-4f35-9882-6ea3c890661b"
            }
          ]
        },
        {
          "id": "44aabfd7-c093-4fcc-9cf5-842d1be96d22",
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
              "id": "c45ca7e0-1b92-4ec8-9a7e-d9a93c834cab"
            }
          ]
        },
        {
          "id": "58932880-f91a-475c-bf7f-cdc44d60b85f",
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
              "id": "09b7b83a-11e8-4bd7-9473-3011f34cb99b"
            }
          ]
        },
        {
          "id": "d3f87b08-dc84-4aa6-b7f6-e081b98df935",
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
              "id": "635812a0-00b8-4764-bb07-b671e5b2bcf8"
            }
          ]
        },
        {
          "id": "be58c057-bb3e-454b-b8da-25ec2597a90f",
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
              "id": "bf103d9d-441b-4b70-ae55-fa2f8922a734"
            }
          ]
        },
        {
          "id": "6ebc4634-f560-46a9-b78d-73a279ba2d40",
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
              "id": "a43a61e9-cc9e-4919-abf9-e5d60236fb2b"
            }
          ]
        },
        {
          "id": "42afcbd6-bba3-41ce-b857-6e590fedcd81",
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
              "id": "a59d3227-862c-4298-9b9e-084bcb62261f"
            }
          ]
        },
        {
          "id": "c6293e50-4c7f-495e-ac06-452a1e00e235",
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
              "id": "de775d43-7f61-433d-abf1-7e32086e0717"
            }
          ]
        },
        {
          "id": "cfe325e1-0b5d-43db-b43a-841e1ab53115",
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
              "id": "a746852a-ae81-481f-a689-913b679df692"
            }
          ]
        },
        {
          "id": "06d3afd3-3137-455b-871a-bb9b6eb721ea",
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
              "id": "10e8aa66-0114-4333-8625-f1d5413d58bd"
            }
          ]
        },
        {
          "id": "3ec22eee-a0c6-4038-8d08-8e254d7e01a9",
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
              "id": "6945a8ab-f3f7-464c-8281-f40633c244e6"
            }
          ]
        },
        {
          "id": "41b2a09e-4132-49a0-b74e-afe8830366f5",
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
              "id": "0452e863-38b6-49f3-b8f4-795986aa4056"
            }
          ]
        },
        {
          "id": "c9ccfcf1-beb8-4d5e-8eaa-6de9c5a645c9",
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
              "id": "2e1f7244-92b4-4884-9b32-c2efa104c54c"
            }
          ]
        },
        {
          "id": "fa29ddb3-4ea9-4e79-84b0-4e8db22ed887",
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
              "id": "3e3d7087-0137-430f-848d-5928c39208b3"
            }
          ]
        },
        {
          "id": "fb165df9-5a20-499b-a8ba-f64a497eda86",
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
              "id": "71e84858-c968-4186-be9c-e76d0d0fa2a9"
            }
          ]
        },
        {
          "id": "2b6e51bd-636c-4a4a-b9be-bc2050e5dc7b",
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
              "id": "bd2f5699-35a9-49a3-9aae-f16f7762782a"
            }
          ]
        },
        {
          "id": "e28cc171-e912-43d7-b4fd-1d04a1e13869",
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
              "id": "c947a8d8-cb69-4f61-a1ed-4515ac75f7ae"
            }
          ]
        },
        {
          "id": "7ef2d9d1-68a0-4632-bd8c-eda289e5c4b1",
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
              "id": "429bb3d4-e17d-4a11-8092-3ef041fefd3d"
            }
          ]
        },
        {
          "id": "6346a1f0-9207-459b-a8bc-ce29b6a9b9b8",
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
              "id": "81895368-6c3d-4ee5-aea9-e836456d8bbe"
            }
          ]
        },
        {
          "id": "4f797465-c2f4-42c1-8a9b-0028577feb0f",
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
              "id": "6ad75b2d-461b-4d0c-a235-2e92edeff10f"
            }
          ]
        },
        {
          "id": "fb8170bc-d7f3-4f03-b53a-f3e8ecf2614b",
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
              "id": "e9ba5362-6636-469b-abc4-2dac774a07ba"
            }
          ]
        },
        {
          "id": "8b598ac2-48bc-4b19-89de-6a141215673d",
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
              "id": "581af5e5-4a32-435c-9b3f-0a221673a0c3"
            }
          ]
        },
        {
          "id": "fdf92a2c-281b-4543-815e-b04b81972192",
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
              "id": "7a892802-c196-4d7a-9dcf-f2acea7725ba"
            }
          ]
        },
        {
          "id": "e41bb940-f8ad-4d43-b684-78bd2e4fef3a",
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
              "id": "06713d02-70ed-4d03-b324-d5906c7e5de8"
            }
          ]
        },
        {
          "id": "8eb327e9-01b8-4175-9c01-60df1b243926",
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
              "id": "f3f3322e-1369-4613-8ae6-72e206de55a1"
            }
          ]
        },
        {
          "id": "0011260a-782e-47b1-ba7f-15acf388a788",
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
              "id": "074bb142-ca4f-414b-b883-aad28ddf933a"
            }
          ]
        },
        {
          "id": "449098a7-d891-477a-82ab-799bdb73ba09",
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
              "id": "f575c449-e6c6-4193-9082-dfd7fb1db42f"
            }
          ]
        },
        {
          "id": "bd90ccb6-6bff-46f9-921f-fdb0e9fb2575",
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
              "id": "6e67b017-132d-473a-904a-c628b9e26926"
            }
          ]
        },
        {
          "id": "b979743c-3a20-42d7-aa01-ff76e6396b2c",
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
              "id": "4916662c-d4ac-4d10-b411-b2c0ae046682"
            }
          ]
        },
        {
          "id": "a578b6c0-32f3-466f-99bc-e770d5895c51",
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
              "id": "7e59aacb-0852-417d-aa34-64b39d8eae55"
            }
          ]
        },
        {
          "id": "b8420c16-b7c6-476f-b51b-8e8f67f89e28",
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
              "id": "6e6a7af4-7141-4219-bd9d-1d7ee57dfe85"
            }
          ]
        },
        {
          "id": "a4e5fbc0-cc0a-479a-a70c-19c6a0d79706",
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
              "id": "09547489-ed29-468c-9353-9262111ecaae"
            }
          ]
        },
        {
          "id": "3cdd886d-d54f-4c0f-8f5e-7461422ca7e4",
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
              "id": "ba0c8a19-3092-4764-b892-a8b720eb27a1"
            }
          ]
        },
        {
          "id": "2b9a7dd1-914e-4c51-9505-93698360ed03",
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
              "id": "1b57cfcf-7cca-4c89-8cb9-8f74f08daf17"
            }
          ]
        },
        {
          "id": "5abf456c-97bd-4955-805b-265b01dc6d66",
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
              "id": "dad16c54-330b-43f5-a0a9-71d902f98a9b"
            }
          ]
        },
        {
          "id": "dc7d214b-402b-44af-b4f1-04de232272c3",
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
              "id": "49984f15-a8e2-4909-9b94-312dcaedd680"
            }
          ]
        },
        {
          "id": "ca60989c-f8df-4469-b8c5-4ca638a6d80f",
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
              "id": "ed394d96-5f12-4e86-a63d-a15ece2cf0ee"
            }
          ]
        },
        {
          "id": "849a948f-dc88-4796-ae57-05140c7759f8",
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
              "id": "4b3346a6-49a0-4533-b464-303e82762640"
            }
          ]
        },
        {
          "id": "5c844a78-a309-4130-9688-d269a9726890",
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
              "id": "f0a0083e-2e2b-46fc-bae2-a5055aa52bf8"
            }
          ]
        },
        {
          "id": "eca29812-6eaa-4dc3-89db-598cf396af76",
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
              "id": "69caf087-bc62-44e6-86a1-361e54ed707a"
            }
          ]
        }
      ]
    }
  ]
}