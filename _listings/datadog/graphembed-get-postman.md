{
  "info": {
    "name": "DataDog API Get Graph Embed",
    "_postman_id": "e230e3eb-f9ef-4151-969b-1a076236a46d",
    "description": "Gets a list of previously created embeddable graphs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "cbca7ebe-b99a-4db8-8388-17f61417d24c",
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
              "id": "988f75a7-a73d-461e-a392-ad84cc830b71"
            }
          ]
        },
        {
          "id": "db20aa27-c5bd-4f5b-bd69-7a598c9ac2d5",
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
              "id": "6a9f9bfc-d774-4a81-ad6b-a413af1f251e"
            }
          ]
        },
        {
          "id": "2b4cb222-e2e8-4e8b-bb61-81e61ab35c7e",
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
              "id": "efd36bfc-82d5-40e1-926f-e69e83682a51"
            }
          ]
        },
        {
          "id": "d90069f3-7d80-4dfa-b322-50ed6ac60d0a",
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
              "id": "0acb38e4-8895-434d-a60b-bf9cfc166baf"
            }
          ]
        },
        {
          "id": "cbc569e3-0519-4d88-bd0f-3ab07c3be099",
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
              "id": "7d16994a-88f9-4552-a874-99ed3f56b15e"
            }
          ]
        },
        {
          "id": "36342e03-fabc-4e0d-a042-54cb19800904",
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
              "id": "a17f0a26-2a95-45bb-8893-c3c677e88db2"
            }
          ]
        },
        {
          "id": "71616379-b6e6-4c68-9b33-faff6764f963",
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
              "id": "21a3a103-9be9-492e-9054-25140a26b5f5"
            }
          ]
        },
        {
          "id": "7798feb4-3411-412a-9a6d-e68b098fb472",
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
              "id": "81e5ceb5-30fd-4eee-94db-9ed0efca5d48"
            }
          ]
        },
        {
          "id": "219ef1f2-6453-47ac-bdd6-2be0c28ab930",
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
              "id": "da7c45b6-53a1-4540-a12e-e9e81feae29d"
            }
          ]
        },
        {
          "id": "c8307b43-91ca-4f83-9f6e-091ca4afaa11",
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
              "id": "a51539f7-230f-462d-890c-8f94e7523beb"
            }
          ]
        },
        {
          "id": "9d7054be-56f9-4355-bbef-76bbce53cfc4",
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
              "id": "1ae19a31-358a-4a60-bb5d-398b7ffca44f"
            }
          ]
        },
        {
          "id": "e684ff7e-f8e8-4bab-b1dd-0e60ba7ade91",
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
              "id": "0f81eda6-1988-45f4-b9f4-c4f631506dd4"
            }
          ]
        },
        {
          "id": "ed8e3a8c-10b7-44e6-9922-f73d37cd488e",
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
              "id": "fddaa959-62f1-44e4-877a-49b89f97a12a"
            }
          ]
        },
        {
          "id": "b8c5f27f-dd87-47df-beec-9ad12cba3f7a",
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
              "id": "aa867183-378b-4dd7-bfa5-6f6fd05322a6"
            }
          ]
        },
        {
          "id": "8c4ade4e-c4df-4fa6-94e6-380c0e6b7d79",
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
              "id": "ce87fd37-e543-4f0c-8f0f-986e88ebfc71"
            }
          ]
        },
        {
          "id": "ffa7056b-3915-4711-95e3-7a66719e1e65",
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
              "id": "d431785e-311a-464b-859b-37d71783c24a"
            }
          ]
        },
        {
          "id": "9e7027f7-6c4f-4cab-af3e-97d09d75aa46",
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
              "id": "d4c5ecc6-9854-40fd-9e7b-caed6447244f"
            }
          ]
        },
        {
          "id": "421b0631-3b3a-4325-a208-5bf17d536b20",
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
              "id": "ed9b97a0-cd88-446c-b957-b7919d2d8fc4"
            }
          ]
        },
        {
          "id": "39af7b44-f7f3-4780-9b97-7abd3abdf345",
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
              "id": "929bb33a-666d-4797-9ffe-5b4942b9725e"
            }
          ]
        },
        {
          "id": "6d97c9c8-eb3a-4892-8387-aa6a4828ea03",
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
              "id": "71f00364-66ea-49d0-9a12-41ccae63b98f"
            }
          ]
        },
        {
          "id": "ba56793b-9623-4bcc-928a-20b6b6b96ba5",
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
              "id": "099348a3-2ba0-40a0-a93c-aea1100533e8"
            }
          ]
        },
        {
          "id": "d2e8f1ad-7941-4809-951e-fa1683e36176",
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
              "id": "3549b739-9fba-461c-aafd-af34221e4385"
            }
          ]
        },
        {
          "id": "67ef37ce-b750-4a08-98f0-45c0ba63dc12",
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
              "id": "0fc353ff-ad48-4b75-8e4e-70373cdac0a3"
            }
          ]
        },
        {
          "id": "f41f93af-c9f9-43dd-9702-1c63bebab36e",
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
              "id": "caf1cd2f-d794-46b0-b67e-d979502f86d5"
            }
          ]
        },
        {
          "id": "4c89aaeb-bdb3-4a57-823d-6419d573acb2",
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
              "id": "89b2f428-947d-4cf1-870c-7e3ece56d6bc"
            }
          ]
        },
        {
          "id": "d1acd868-c0d6-47f4-892c-23e1e493fd74",
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
              "id": "d3fefae5-fcd1-45e5-a52b-396f900d4a3e"
            }
          ]
        },
        {
          "id": "b18f3e0c-a382-49ea-bb8f-31cc202816ad",
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
              "id": "fa324f33-a2a2-47bf-ba3c-276ee01b5dc7"
            }
          ]
        },
        {
          "id": "90d260e9-9744-45f7-95af-0d4703fa041a",
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
              "id": "e948da6c-efc3-45f0-a440-eed1b884daea"
            }
          ]
        },
        {
          "id": "6a75805f-76f9-4fc4-bf41-e0b1c0586f00",
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
              "id": "d3b93631-7151-4373-9a12-7915a66fcc7d"
            }
          ]
        },
        {
          "id": "bdb95810-29c6-4952-a052-21664d996cbf",
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
              "id": "2c69619e-e13a-4c80-a6b7-a0d286427e7b"
            }
          ]
        },
        {
          "id": "31827e5a-523f-4878-b8f4-e6fcdb08616c",
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
              "id": "31d32cf6-ac98-4f57-874b-dd8e62cdccb4"
            }
          ]
        },
        {
          "id": "9e1dd9a2-21e2-423f-8873-920a7cf1afab",
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
              "id": "414c79e9-6aa5-4eca-b8bf-3f6ed727e6f2"
            }
          ]
        },
        {
          "id": "3eb541ec-0d04-407f-9438-17f468fdde10",
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
              "id": "82dd03d3-6604-4397-aec7-2b8cf7166e27"
            }
          ]
        },
        {
          "id": "81ff375f-2a16-4064-ad84-72acc6c0260a",
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
              "id": "dc29de80-2f16-4d12-877a-37c9d079cb0d"
            }
          ]
        },
        {
          "id": "7b5c69d1-1053-465b-91f5-708b2309e0ea",
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
              "id": "c02b6a26-0a86-409e-9b2c-734d507c1704"
            }
          ]
        },
        {
          "id": "40d22a35-03c4-4257-89ea-2d43d9d46a66",
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
              "id": "84e951d9-2ac7-4526-8af9-ebcbedda7cb4"
            }
          ]
        },
        {
          "id": "0197f387-2ded-4b47-9c2a-d37316e9b804",
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
              "id": "5adabd32-cf29-4173-86da-07317bfadb52"
            }
          ]
        },
        {
          "id": "12d58c5b-7ac3-4395-81bd-135a70a92fd0",
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
              "id": "91affc9b-8319-44d2-bcd9-0b803e53bb7f"
            }
          ]
        },
        {
          "id": "933598da-a8fd-4e1f-922a-ad8be2864ebf",
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
              "id": "2fea8705-4ee3-4e12-8f9f-d2e158aff007"
            }
          ]
        },
        {
          "id": "ad109dcd-3f84-42f8-acb4-ef23abfc2c05",
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
              "id": "5f1bd78f-6def-4377-87c0-d6b91e21ff9b"
            }
          ]
        },
        {
          "id": "254b5abc-4b25-4c06-834d-d23fdd272c86",
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
              "id": "8217e436-3755-48ec-9e25-3519655d944c"
            }
          ]
        },
        {
          "id": "353ca621-9d91-4d76-9148-16c98cf54c1a",
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
              "id": "749f6092-ac9d-48ce-ad82-2620961ff89a"
            }
          ]
        },
        {
          "id": "5a7be089-9208-401f-9b3f-9373f78bc561",
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
              "id": "bf0583de-3dca-40a0-8a5e-65b250c7d6ea"
            }
          ]
        },
        {
          "id": "2c117298-d6bb-4276-bc1d-170b0df95e59",
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
              "id": "abe4a3c2-e5a4-4ee9-95fb-59db825667dc"
            }
          ]
        },
        {
          "id": "485afa8a-f5a8-476b-b322-393eb25abdc1",
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
              "id": "e617eca5-bf1d-4e4d-b503-560a02cc00d3"
            }
          ]
        }
      ]
    }
  ]
}