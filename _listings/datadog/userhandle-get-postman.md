{
  "info": {
    "name": "DataDog API Get User Handle",
    "_postman_id": "d7567612-e90b-4e5d-bb1c-4a107af560b9",
    "description": "GET user handle",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "03c47f9d-8e57-4673-8e97-af91f01c19a0",
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
              "id": "b9120bd0-7081-4305-907c-ca4e5c523ddd"
            }
          ]
        },
        {
          "id": "36ca36c4-50f4-4c3d-8cb4-2ff1453335f5",
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
              "id": "91660430-1b06-45b2-a51b-48f7ca7cc26a"
            }
          ]
        },
        {
          "id": "4d1186da-8055-4d1f-9da9-8f4948cd1bd0",
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
              "id": "a99cb7ef-e0d5-42e9-8cc7-bc289dbb0c4a"
            }
          ]
        },
        {
          "id": "494ae935-7a59-4bd2-aee7-585e7ae41939",
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
              "id": "68c42a21-fee2-4318-8bcc-1f116454e233"
            }
          ]
        },
        {
          "id": "95b886c1-ad4f-48a8-8c3d-bdd9209bbab9",
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
              "id": "00996084-170a-487a-aefe-3ade1df8af5d"
            }
          ]
        },
        {
          "id": "0ee01530-a574-4b05-890d-3fcfb5819927",
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
              "id": "e20bacaa-7ab7-427d-86b1-60bd836e706f"
            }
          ]
        },
        {
          "id": "64eb6274-6834-4409-af46-71478916c469",
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
              "id": "19af1df8-e52d-4cca-9bd2-c85c9f8dcc7d"
            }
          ]
        },
        {
          "id": "fd5a49fb-4114-4283-91e6-0fa4f4f91b0b",
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
              "id": "5338d3e5-3b71-4248-a5ad-be21f7d71471"
            }
          ]
        },
        {
          "id": "b034c507-370a-4d60-b550-624ca121523a",
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
              "id": "40fba5c8-1405-47e6-90de-09025a5a0263"
            }
          ]
        },
        {
          "id": "770a54be-640a-4208-9544-623a1785d91f",
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
              "id": "a45f73a9-5234-4ae2-a7bf-ef1fabb8f0bf"
            }
          ]
        },
        {
          "id": "f541b8bb-edcc-456f-a22c-64034184bf6b",
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
              "id": "685ffaa3-9504-4323-8ebc-cc0b6c95682b"
            }
          ]
        },
        {
          "id": "dafb28e4-8afb-452d-a6e9-bb556c69dc27",
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
              "id": "9ccca438-24fd-4fbf-aa67-1e192d872113"
            }
          ]
        },
        {
          "id": "55dd5f06-a5fa-4074-94c7-8c1324d18d53",
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
              "id": "06f32292-b363-4540-8f7e-3e179f2159c0"
            }
          ]
        },
        {
          "id": "ca6f55c5-6bef-45fd-9324-5a3dffba38a5",
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
              "id": "b206d4d3-0b42-451b-a157-77e8b90e7450"
            }
          ]
        },
        {
          "id": "1448a845-6102-4c99-8cd2-2a496aea19f3",
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
              "id": "dc342804-4d46-49c2-ba70-2cd7fb833236"
            }
          ]
        },
        {
          "id": "cb95d9ef-5822-46a1-a16b-0e2c8496101b",
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
              "id": "40c3b7c6-90bc-4e14-87b8-bcedb799d78e"
            }
          ]
        },
        {
          "id": "a55e1579-ce33-4e47-bb0d-62235f649f23",
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
              "id": "fd9e4113-b42c-4928-bd82-5f21bad21b5f"
            }
          ]
        },
        {
          "id": "681aca75-8daf-4b56-aea7-d5464b347262",
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
              "id": "e607f852-493f-43c9-99db-d91c37a6bb01"
            }
          ]
        },
        {
          "id": "f5b8c4fe-4e02-4678-adae-3003e9af7dc9",
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
              "id": "9e39fa94-fbb6-445f-877f-630dd43190ef"
            }
          ]
        },
        {
          "id": "11316866-9be4-4283-9faa-bad93759d265",
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
              "id": "3e28b1fe-620a-4968-a180-f7c95a38a3c6"
            }
          ]
        },
        {
          "id": "23b74e23-31b4-4fce-8649-9460b02188f4",
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
              "id": "9c76b27d-a8c5-443c-99e7-2c15a6167e94"
            }
          ]
        },
        {
          "id": "c592254b-9280-41d0-900b-f946b68ec568",
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
              "id": "a9368c3f-d60b-4b8a-8ad3-c4e1baad0237"
            }
          ]
        },
        {
          "id": "703167e5-d6be-4adb-a8d5-b04ce386aaa3",
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
              "id": "d206c8e4-7d0a-4c67-872a-4f8f6dd14837"
            }
          ]
        },
        {
          "id": "b86acc5b-896f-4c50-968c-332a6eb6f6b8",
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
              "id": "9cf34d34-e120-4d02-a9d8-c7b479a6c5c2"
            }
          ]
        },
        {
          "id": "aa81fd85-2956-48c3-8658-ec395af96b75",
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
              "id": "039f18cb-78bf-4049-bea1-9bfa80900482"
            }
          ]
        },
        {
          "id": "1f981594-c698-4349-95d0-d1dfbed03959",
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
              "id": "8a240cb3-c5ba-460e-a0f2-5408845178fa"
            }
          ]
        },
        {
          "id": "e8f7be96-a6ff-40ec-8895-e021a08c27ac",
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
              "id": "27100811-0ade-4581-bc8d-fb7f379c4604"
            }
          ]
        },
        {
          "id": "76fa6b2a-d6b0-4819-a272-3f765a6c0935",
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
              "id": "32215db3-ab48-4257-8ee0-07dbbd528d32"
            }
          ]
        },
        {
          "id": "683b2f32-7cf7-4fb1-bbc6-c899931ed742",
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
              "id": "3799506d-b70c-449a-be32-847b1248e60d"
            }
          ]
        },
        {
          "id": "2f95584d-3e1a-4fec-8aa1-6449baab05de",
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
              "id": "0ab0dc04-2eac-44d0-b621-7c6dac364342"
            }
          ]
        },
        {
          "id": "a66281ad-b84c-4f9d-8910-c7ce1cd4b301",
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
              "id": "b936ef9c-a87c-48fd-b533-450cc0580631"
            }
          ]
        },
        {
          "id": "1ce655dd-149f-4f8f-a033-6ff38ea668ad",
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
              "id": "ba7e53ee-a54a-4171-970c-bf41a01d2a1a"
            }
          ]
        },
        {
          "id": "53cb4bf3-6e5d-4bd1-ac97-f77ff4158d31",
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
              "id": "60aab22c-8ef8-4b35-97f5-988c1be5c441"
            }
          ]
        },
        {
          "id": "f041dc6a-aaf2-4204-b2f8-a2198409c14b",
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
              "id": "3323177c-d1ac-488d-9618-1ce97902c985"
            }
          ]
        },
        {
          "id": "0bbf4aa0-4ea0-43b3-801d-01ecdeb8bbe2",
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
              "id": "6bed45a2-264a-43b7-8fe1-ae419a3d562c"
            }
          ]
        },
        {
          "id": "2781dccb-82d9-45de-bf97-db3d6abf513f",
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
              "id": "0ca7331d-a54f-446c-8c98-6b8cdcd58210"
            }
          ]
        },
        {
          "id": "ef2ff353-4e3c-4e88-9512-dffe4ff86dd3",
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
              "id": "444a5bc0-cea6-43a3-9ed2-486e865fef8f"
            }
          ]
        },
        {
          "id": "2a27b421-6764-48f7-8b4c-600c564ccf47",
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
              "id": "12198606-cc73-49c4-8c74-ca398fb1b0ed"
            }
          ]
        },
        {
          "id": "500fcc7c-a3a6-4072-a209-6e01612050ad",
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
              "id": "10ad5be5-d433-4576-b3ba-553b87c3dc19"
            }
          ]
        },
        {
          "id": "1c8a7552-35b5-43dd-9580-bc05013b96fc",
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
              "id": "c48fc2dd-dd23-49a6-88ad-3d18d0e448ce"
            }
          ]
        },
        {
          "id": "a1252d07-afb0-4e9e-be04-298f1c0d7ae0",
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
              "id": "705cce75-64cc-46dc-a13f-9e223be3f137"
            }
          ]
        },
        {
          "id": "b70f2968-ae15-4286-9016-a9d6f0acd5d0",
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
              "id": "a0c4f1ec-51a5-47a8-8f46-86ba35d4d375"
            }
          ]
        }
      ]
    }
  ]
}