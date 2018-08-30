{
  "info": {
    "name": "DataDog API Delete Dash Dash",
    "_postman_id": "09e7458c-c020-4e9d-b675-ea02d3c71960",
    "description": "Delete a Timeboard",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "16381673-f1a8-4fc6-a41a-84e3da360a99",
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
              "id": "7fc4481c-e807-4d96-9d50-b635bb868569"
            }
          ]
        },
        {
          "id": "a101cd2c-51ff-4b3d-a199-7428c63f881a",
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
              "id": "e8f0d6bb-9d2f-492c-81be-7599899d41d5"
            }
          ]
        },
        {
          "id": "22c7fe6f-4499-4577-a86b-957fce9d7fc5",
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
              "id": "bd2e7c5a-7488-4bd8-a782-1b6e62c09555"
            }
          ]
        },
        {
          "id": "7baa2da1-f48f-4fbd-8f8a-72445abea9e7",
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
              "id": "6df38ac3-7594-47ad-9aa1-51442c56afcf"
            }
          ]
        },
        {
          "id": "0319111c-22a4-4b35-90dd-69b7a88b94b7",
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
              "id": "2053a6d4-f1a2-4257-b77f-6e9230c7f71b"
            }
          ]
        },
        {
          "id": "f6611e1a-5480-434f-b92e-82e7f63d35c8",
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
              "id": "172ea9a9-6598-42ab-88e8-0dca38defe78"
            }
          ]
        },
        {
          "id": "728fdade-73c2-440c-96ea-0a861b9f9e12",
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
              "id": "32a4f647-4235-4a6d-8a60-27fe77f3c408"
            }
          ]
        },
        {
          "id": "702b58e2-ecfd-44a4-a912-1fc53d0ee0f4",
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
              "id": "76eaa5e2-d513-4630-8a3e-367892ab8e02"
            }
          ]
        },
        {
          "id": "15ea3980-4a15-4776-bb3e-da4fe13d1989",
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
              "id": "8af14caf-57a3-43e8-b1a5-0750e3794010"
            }
          ]
        },
        {
          "id": "e7bc2320-5ecd-41c7-b2ef-a0790ac88d5b",
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
              "id": "8757a0e3-e723-4f68-bd6f-60280f785892"
            }
          ]
        },
        {
          "id": "e35638ce-ea34-4a77-bf5b-ba1d2fa61c16",
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
              "id": "98f89f71-d9df-4f07-b971-24b8c620b3a9"
            }
          ]
        },
        {
          "id": "14b9169a-127e-49f7-879f-b7e47aa18b64",
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
              "id": "a7db88ba-9ce3-459a-b423-b7889d20f947"
            }
          ]
        },
        {
          "id": "4e993306-46c0-4d63-bc88-6a7eb6d32364",
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
              "id": "ecb276e4-8d05-4518-822e-abf642381ea5"
            }
          ]
        },
        {
          "id": "30ad51b3-c5d6-46d3-9827-aa1b6dbffaf3",
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
              "id": "7b9e8daa-e37d-4f22-91a7-9f06a655be1d"
            }
          ]
        },
        {
          "id": "4bc4a4d6-c0a0-4c8a-bb40-754cabf98b87",
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
              "id": "2ed627e7-7bea-4e22-907f-53ced7435508"
            }
          ]
        },
        {
          "id": "c428f82a-d403-4d50-a9b9-253ba616a98f",
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
              "id": "239ef891-cd68-4ec7-b198-64fbc6496115"
            }
          ]
        },
        {
          "id": "6d28f1f1-9202-4908-adda-09a138bdafea",
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
              "id": "06b1b44a-72c6-4c3c-b627-67fce7398923"
            }
          ]
        },
        {
          "id": "fad1caa8-1d9a-40d8-abcc-4caab4759fb1",
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
              "id": "f5408479-b452-4fbe-982f-61c7f6e8dfde"
            }
          ]
        },
        {
          "id": "3abbde9a-1646-4819-a9fe-b281428d5567",
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
              "id": "681990a1-927e-4858-9096-8f52785e53f8"
            }
          ]
        },
        {
          "id": "d099dbe0-f81d-405b-aeb8-2172322ea733",
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
              "id": "db755ba5-8f56-4239-afd3-85ff08c105ad"
            }
          ]
        },
        {
          "id": "c75a8de1-2866-4fbf-9ba0-252e55f752ee",
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
              "id": "14ec6eb5-6d2d-495d-b320-9646ddc79eb2"
            }
          ]
        },
        {
          "id": "44b78ba1-e0b1-4e2d-b2bf-2b24d75806bd",
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
              "id": "b386d9b9-d211-4477-a350-934017711c1b"
            }
          ]
        },
        {
          "id": "fe76c361-4d65-473c-ad22-df74e896449e",
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
              "id": "c23a26f0-050e-4ed9-9cde-02247226ed48"
            }
          ]
        },
        {
          "id": "2096105e-76d8-4366-8526-eb12c923a103",
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
              "id": "392061d1-007b-4130-af21-2fdb71e93dc6"
            }
          ]
        },
        {
          "id": "f2c1ccf4-eca1-491b-b274-8445a1f6d285",
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
              "id": "cc39eb7a-6b43-4ff0-9eed-9c6e79a8225f"
            }
          ]
        },
        {
          "id": "6ac28702-1056-4dff-b13c-e51b7c0c4b0a",
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
              "id": "67df8cdb-d54c-42bb-a8ba-d6cdcb6a5c09"
            }
          ]
        },
        {
          "id": "471ca9eb-0452-42f6-ac44-397e3295ca1e",
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
              "id": "6707ccc4-1738-43d6-9e4f-da073aa6b37c"
            }
          ]
        },
        {
          "id": "72c41d75-07d9-4947-ab39-c589b22baabc",
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
              "id": "4601eaa1-d8c5-443c-9d05-71a422a8ef19"
            }
          ]
        },
        {
          "id": "6a2782d0-63d5-40f3-bc29-b83cec98f330",
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
              "id": "22baf25f-8d57-4122-a6ee-fb513d2f5ae8"
            }
          ]
        },
        {
          "id": "81b53d19-9725-4d32-a64e-03cc88036dc5",
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
              "id": "85ff67e0-c0de-4477-b149-fac5ade3e229"
            }
          ]
        },
        {
          "id": "035774a5-c763-4d41-846b-d43b2ab00b82",
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
              "id": "214b7362-9cae-4267-aa66-3801f2618142"
            }
          ]
        },
        {
          "id": "aa0c2c9f-64d7-42f0-8edd-ec0aac5b53be",
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
              "id": "56523181-cc93-41ab-8f66-992749492519"
            }
          ]
        },
        {
          "id": "479b091d-9fcd-4422-878e-b1cec8594021",
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
              "id": "8829c769-09e2-42db-8de2-cd1697e45586"
            }
          ]
        },
        {
          "id": "230f97bd-7790-4353-8701-51c03084a53a",
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
              "id": "0a40056d-ac4a-4f77-b8bf-fc6334f6d7de"
            }
          ]
        },
        {
          "id": "3c8573c2-4f51-43da-8824-09bcdb8805c4",
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
              "id": "76502b21-432b-489b-8715-493348b8b633"
            }
          ]
        },
        {
          "id": "edb8ac4b-7d4a-47e9-92de-23f5c9e883ee",
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
              "id": "a3079cff-2c26-4b33-b292-dfe3d72c8d0d"
            }
          ]
        },
        {
          "id": "33c1b3df-fff9-47fe-a82c-d9a680bd0cb7",
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
              "id": "483d221b-b282-4b42-a703-96f85b81d778"
            }
          ]
        },
        {
          "id": "88227cf7-1139-4ea5-bc5d-3a25d299937c",
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
              "id": "f550bbbb-0a4a-449e-9bde-2c7557bf4b55"
            }
          ]
        },
        {
          "id": "1c076215-1adb-448c-b0fb-9258e9f0e170",
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
              "id": "8261b2c5-4a81-46a0-b1ab-04b974c5cc19"
            }
          ]
        }
      ]
    }
  ]
}