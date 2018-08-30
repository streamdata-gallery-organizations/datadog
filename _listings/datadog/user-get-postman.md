{
  "info": {
    "name": "DataDog API Get User",
    "_postman_id": "2f400982-dc29-412d-9708-f2f98661530e",
    "description": "GET user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "d6029a9a-8a1a-41b9-8ad5-d4e41a50992e",
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
              "id": "5d4e46f5-7285-4733-9578-a506fbaf8227"
            }
          ]
        },
        {
          "id": "f76af9fa-3401-4b6c-ae81-488f1434284e",
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
              "id": "d1d6ff17-49fa-454f-b3f9-c3a10a623e7b"
            }
          ]
        },
        {
          "id": "bc79d2a7-67ed-4c8d-af3c-d06c6e78cd35",
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
              "id": "c27db667-1060-473b-af1b-ecd181846857"
            }
          ]
        },
        {
          "id": "0154e354-6cde-4ead-9394-727a2858eb2d",
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
              "id": "b9f62873-ee10-43fe-8c61-458a3e1c4f6d"
            }
          ]
        },
        {
          "id": "3ea326d5-f00c-47fc-94a0-a49de2d6e705",
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
              "id": "238d9e40-7f64-4707-840f-7ef623a84e0e"
            }
          ]
        },
        {
          "id": "2e3bdffb-ca41-437a-82c3-7170c5a5af10",
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
              "id": "6eefdea5-cd9a-40cb-b15d-9c4f2f5de1a6"
            }
          ]
        },
        {
          "id": "92d7b93a-23b5-4ac8-8afc-08d3ee04df90",
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
              "id": "ce1779f1-76f7-4c3a-b86b-1bb245f1e531"
            }
          ]
        },
        {
          "id": "8df132a0-1284-467a-9172-629fbff2e3ff",
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
              "id": "bdc10bb5-18ef-44eb-98ef-6870f7c583df"
            }
          ]
        },
        {
          "id": "178af101-bd17-45d8-b4ce-248f3f0d3342",
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
              "id": "bb9423da-dd02-4092-9655-fb6619292b6c"
            }
          ]
        },
        {
          "id": "ddf4a91a-b784-4af0-8955-121d6a19f4f9",
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
              "id": "ff8f759a-e4b6-4bd2-83f6-522c02acaf5d"
            }
          ]
        },
        {
          "id": "6ca1b8dc-6cd0-40bb-a715-c352b29eac3a",
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
              "id": "e8bf939f-6298-48d0-b810-ae96708f8890"
            }
          ]
        },
        {
          "id": "4511e945-2b07-4094-a6da-830e4152e9b9",
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
              "id": "50917d45-ebdb-440f-afb1-21c2332e1d9d"
            }
          ]
        },
        {
          "id": "1661939c-5549-4def-b99b-c52817943f5d",
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
              "id": "d1e72ae2-f3f5-4a51-9f4c-f92177c28787"
            }
          ]
        },
        {
          "id": "bbc12fd9-3b9d-4633-ad15-bf39d9f7a686",
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
              "id": "fe4bd2f6-e74f-42bd-bbe9-bc5cc1c050e8"
            }
          ]
        },
        {
          "id": "c7e0390c-359a-4c41-8ad6-9d3ea04b8d5c",
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
              "id": "48b7b451-ac84-4f8f-9567-a16ee627812c"
            }
          ]
        },
        {
          "id": "06d471ac-15d6-4abc-b56b-19c3cb08ccd3",
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
              "id": "c8fa4276-a5f2-46be-a545-8ddf71d3b43d"
            }
          ]
        },
        {
          "id": "e70658d8-e498-4721-b37e-b5392fa573c1",
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
              "id": "05be4e49-c46a-45f0-8e6b-b7b20769ab86"
            }
          ]
        },
        {
          "id": "24f3ea20-23ff-436f-b049-c584beb783e2",
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
              "id": "bedd81be-4296-4375-96d2-df576aee1690"
            }
          ]
        },
        {
          "id": "735e2173-846c-4da6-9acd-a42f3408b0fc",
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
              "id": "ed757d49-15e8-480f-8a91-96940b9f0885"
            }
          ]
        },
        {
          "id": "da6ab91a-2ba7-49b2-bb9e-bad5c1fae9a9",
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
              "id": "802fa0a9-3443-45cc-b12b-f80e1089850d"
            }
          ]
        },
        {
          "id": "2fee3d5a-15cf-497b-ad6c-29db9fc2e317",
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
              "id": "be83d73b-81d7-4bb6-97f5-b74254d235b7"
            }
          ]
        },
        {
          "id": "495a7282-7359-452d-b92c-c1bea1017eb8",
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
              "id": "0f0fb642-f9a6-4956-85c7-25201f8e1b22"
            }
          ]
        },
        {
          "id": "a6509ff1-5c19-4e61-82c1-9bec5bbfc2f1",
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
              "id": "3da17c02-6cec-4212-8ebe-8177d828cf2a"
            }
          ]
        },
        {
          "id": "8a6042b0-22d2-4e05-91b6-9d8e45bc8625",
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
              "id": "d7388c92-8fc9-4c5c-9efe-969d9e93993a"
            }
          ]
        },
        {
          "id": "6b91c1a6-e909-49cf-9ce2-4b6f4e2f2b4f",
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
              "id": "d68fa6c4-6165-4d74-a0a2-d93412a2e68b"
            }
          ]
        },
        {
          "id": "9084c0a0-a0be-44cc-bc44-3d63767ed584",
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
              "id": "07d1986a-2ed8-4866-81d1-5e9c211986cf"
            }
          ]
        },
        {
          "id": "aeeb108d-1a0f-4f82-8f96-90ea493499a3",
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
              "id": "b38ec41a-8349-4ccf-b973-81ffd8193313"
            }
          ]
        },
        {
          "id": "002476d1-66d6-4278-868d-d07395664840",
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
              "id": "e8ece131-7920-45d4-96fb-5db112408758"
            }
          ]
        },
        {
          "id": "0183c0f0-73a2-43ba-b91a-33e0b912da56",
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
              "id": "fb9e9df0-4ccd-4f16-9fb0-7eb73e42138c"
            }
          ]
        },
        {
          "id": "b154cca9-ca81-44ff-9744-2854451c630f",
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
              "id": "7a28d9be-7968-4d34-b142-7702d7bfda5a"
            }
          ]
        },
        {
          "id": "b1df39e5-6abe-4e78-b79b-466cec908aef",
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
              "id": "35ffcb53-70a7-4ab9-9a9a-28f282008ee6"
            }
          ]
        },
        {
          "id": "cf729877-dd80-40d7-9645-f58a1457ae93",
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
              "id": "5e63f37c-fd4e-4127-b8c3-2d72e3cf21ac"
            }
          ]
        },
        {
          "id": "a420eaf8-d963-4a91-afc8-e94e9fde0536",
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
              "id": "ad82eead-61f9-4946-901f-4f2359fba051"
            }
          ]
        },
        {
          "id": "b375a72c-aff7-4e81-8ad0-a158a51a3b67",
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
              "id": "20bce25d-28de-4bbe-aec4-13ba3c646f20"
            }
          ]
        },
        {
          "id": "86294154-77c8-4fd7-b16a-c6f4f2f07d20",
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
              "id": "d3d1d8eb-691e-4d5c-ac1d-f15e91e601b4"
            }
          ]
        },
        {
          "id": "ccfa0a66-5d73-4705-9133-cd74a4f89bf1",
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
              "id": "85acc666-24cd-4df7-abc1-3d8619644a83"
            }
          ]
        },
        {
          "id": "0130d206-9029-4be9-a7a2-a24c2f6f2c91",
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
              "id": "b9b5bfe7-28f4-4813-a055-58652634bc5e"
            }
          ]
        },
        {
          "id": "368de54c-ed79-47b6-9d53-41bd125fb113",
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
              "id": "05f6fde0-a8d7-4d90-aa7f-94a5951534c3"
            }
          ]
        },
        {
          "id": "0f64ce34-38d2-4d26-b5ff-6f20adfc78b4",
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
              "id": "c9d1a415-6e0d-43ef-8bfb-31b8cf1e7c8b"
            }
          ]
        },
        {
          "id": "b9b4e8b2-4ff2-4ba7-8680-2e7ea6836579",
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
              "id": "fe183ffb-b377-4e22-bf2d-5a9c91f5ddc6"
            }
          ]
        },
        {
          "id": "64994c99-1070-4295-8d2b-c9bb2e5da7ae",
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
              "id": "9b3f60ff-f794-4891-b4f1-8390535c29e2"
            }
          ]
        },
        {
          "id": "a79c8b75-47ff-47ea-b0c2-e97c185637ec",
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
              "id": "9f1a1eff-b979-4536-9b2c-1280468f167d"
            }
          ]
        },
        {
          "id": "99f883d3-f3f1-4f67-9827-70a46b91a719",
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
              "id": "0948dc70-4030-4491-bda6-5022003adb2e"
            }
          ]
        }
      ]
    }
  ]
}