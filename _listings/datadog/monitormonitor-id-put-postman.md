{
  "info": {
    "name": "DataDog API Put Monitor Monitor",
    "_postman_id": "a8c85546-fbff-40f1-8967-814e57dd605f",
    "description": "PUT monitor monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "b9d6670d-c0bd-4af4-9fd2-3f3374661052",
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
              "id": "69e1c5ff-c506-4f54-b516-a7e725ee359b"
            }
          ]
        },
        {
          "id": "5e53f4f9-218d-4481-bec0-640e25e0a21f",
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
              "id": "798bb095-1d74-4956-b2e9-ee8e07fde800"
            }
          ]
        },
        {
          "id": "12d92def-dece-435d-b93e-eaed69336998",
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
              "id": "0f6cf6c5-1395-42ca-b5e5-fd6c3e6d6159"
            }
          ]
        },
        {
          "id": "bc58672e-73b7-4727-b5b3-0045deedeb38",
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
              "id": "5f8b0470-479a-4599-b3f5-2e0775bf2dfa"
            }
          ]
        },
        {
          "id": "373d4729-b59d-450f-b1e1-f7713db0fd1e",
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
              "id": "0c874929-81f9-45bc-a90c-30f19d1d3a7d"
            }
          ]
        },
        {
          "id": "84db7661-3af3-47da-8d0e-b5a64f77ad08",
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
              "id": "09d0bf8d-b466-4f4e-9e8e-06a0bd1dfbcf"
            }
          ]
        },
        {
          "id": "9f89e27a-17db-4197-b839-92c3fc7a0c37",
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
              "id": "f1f55e84-ddde-4d17-b90c-66af1052edfb"
            }
          ]
        },
        {
          "id": "7b7b101e-fec8-4783-bba3-b231e8a1869b",
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
              "id": "a9bbefee-5273-4787-a24e-2a523b1cdf94"
            }
          ]
        },
        {
          "id": "8f638eb4-acf3-4d63-8931-913a216c44ac",
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
              "id": "3c199f3f-2402-439e-b840-ba744006932d"
            }
          ]
        },
        {
          "id": "555c69de-9897-4b0b-a5fa-9950563f7aa9",
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
              "id": "e7162d41-070c-4012-a2dc-a01d3393c2a7"
            }
          ]
        },
        {
          "id": "0bfca539-63ad-405f-99af-3a384476e4cc",
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
              "id": "7368adb8-b2a6-406f-95db-ab97b362d4fd"
            }
          ]
        },
        {
          "id": "4d496fe5-df98-4cb0-9bfc-cb37f57df9da",
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
              "id": "3e2404a2-3810-44b2-bd54-e27fb453a2df"
            }
          ]
        },
        {
          "id": "1dc82008-4198-455e-95e0-bf86a2b480d6",
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
              "id": "c8f1edb5-ea42-42f8-94e6-eecbf066f616"
            }
          ]
        },
        {
          "id": "d0878428-e86e-4c5c-8f87-69864a731f84",
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
              "id": "e4ae862b-cb63-468b-bffe-96973cdc7e82"
            }
          ]
        },
        {
          "id": "0f50478f-8efb-4b40-8c98-21f00957e94f",
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
              "id": "4755c363-a759-4943-bf30-e81f2b5e3918"
            }
          ]
        },
        {
          "id": "7f13168a-0209-40d6-a261-aa79cf3939c9",
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
              "id": "6f2cfee5-7579-425a-acda-2dce9c8ec6e1"
            }
          ]
        },
        {
          "id": "2a62788c-d943-4228-b025-079b79413824",
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
              "id": "0e79071a-20b4-4964-8f37-9318d7d0d1a4"
            }
          ]
        },
        {
          "id": "75bdfdd7-f7a3-40fa-90bf-79aaa0a2a623",
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
              "id": "127fcf91-5de7-450b-9065-0e895d04cf93"
            }
          ]
        },
        {
          "id": "593f1494-f37d-4a0a-b90a-4b092486fcb6",
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
              "id": "9f62aaf9-671f-424d-b18e-ac9d48a1e5a1"
            }
          ]
        },
        {
          "id": "c3229653-9fea-4938-97ff-212fcdd1a7d9",
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
              "id": "87534a57-702e-433a-ac62-f819b5380320"
            }
          ]
        },
        {
          "id": "8d7480ba-5047-471e-92cb-77970e4cd6ab",
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
              "id": "89e565e2-35ec-403a-af8f-87705122b8a4"
            }
          ]
        },
        {
          "id": "293faa17-b9ae-4753-9f97-86f38b468f42",
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
              "id": "65768a65-85c6-4eff-b624-a0497e1dcc3d"
            }
          ]
        },
        {
          "id": "fbb0e572-bfee-4c98-8ed3-7b8d777c43f1",
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
              "id": "f1abf72f-52ac-437f-9f92-56213a8537bf"
            }
          ]
        },
        {
          "id": "e29e3d2f-b0cc-458e-9004-e7732deaa880",
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
              "id": "f7d5f1e3-9a5f-4377-a39f-7490bcf2f3d7"
            }
          ]
        },
        {
          "id": "98127353-cb32-4ad5-88eb-4c604a1d8834",
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
              "id": "5a3a5171-185a-42c4-abb2-619899200000"
            }
          ]
        },
        {
          "id": "a282aa15-0d7f-4141-ad26-130e9e28f45a",
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
              "id": "9ee8654a-1ab1-49e5-bf22-3ab29fb80f8d"
            }
          ]
        },
        {
          "id": "0e4f90b7-16fd-4baf-a2d5-80cdcaa7d1d5",
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
              "id": "08e3bcff-f045-46e8-b087-f1f3df7b790c"
            }
          ]
        },
        {
          "id": "39ad2ab3-8c10-4a3b-bf37-17c260493b53",
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
              "id": "19c34766-0e39-439c-a0fc-6bb97f420b48"
            }
          ]
        },
        {
          "id": "673c9628-a7a5-4992-88c2-463164cbf539",
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
              "id": "99de32ab-4768-491f-bbcb-8add7263667e"
            }
          ]
        },
        {
          "id": "e7dab9cb-3aae-4d51-8e4b-659567ded001",
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
              "id": "78973198-a727-463b-a72a-b2fced6e0c90"
            }
          ]
        },
        {
          "id": "6c6e5bec-8dd0-4d6d-8c1c-27ccc146f5ae",
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
              "id": "acc29ab1-4c7f-4ec0-ab17-eb2f37409063"
            }
          ]
        }
      ]
    }
  ]
}