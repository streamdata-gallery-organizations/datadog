{
  "info": {
    "name": "DataDog API Add Monitor Unmute All",
    "_postman_id": "baed5bb7-33b8-4178-b580-0b292a88d675",
    "description": "Disables muting all monitors. Throws an error if mute all was\n        not enabled previously.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "5ad2e8c9-0418-45e9-a0da-b0196c8eff38",
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
              "id": "4cdd7551-7195-42ee-95cf-4ff8c744b301"
            }
          ]
        },
        {
          "id": "19b92ca6-1e24-4229-a4c4-6e5ce623ec71",
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
              "id": "b1792ebd-89a5-4d90-844a-c374cb18c06a"
            }
          ]
        },
        {
          "id": "59508687-f2d4-430d-86ee-78e224766a38",
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
              "id": "74e379b1-8a48-4c72-96eb-3e0aa4cdbe9c"
            }
          ]
        },
        {
          "id": "877fafe9-17bf-48bf-9856-33b34d4e4422",
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
              "id": "167a18b7-760b-4a0b-a350-78e7030b511b"
            }
          ]
        },
        {
          "id": "fa92a15e-f041-4f64-9d32-bd5472909106",
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
              "id": "9af054da-c7cb-436a-a58f-b1afffb94eb5"
            }
          ]
        },
        {
          "id": "d33cffd9-aeb1-4ed5-91d6-2ddc02b10a17",
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
              "id": "fad55b6a-0fbf-4fcc-ae53-5634269b9acd"
            }
          ]
        },
        {
          "id": "389bbd33-4658-47d4-84c0-45d00e325cf4",
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
              "id": "a33e8f92-d7b0-486d-ab91-ca8c8b06d509"
            }
          ]
        },
        {
          "id": "79063597-4a39-4ce1-a428-0e1728061ce0",
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
              "id": "b148ffb5-d337-4184-b395-af8f0904ef26"
            }
          ]
        },
        {
          "id": "03e01739-076f-4131-9e62-3f86ea17b839",
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
              "id": "8ed5dae1-3cb5-40cc-8d7a-099a0ec2fed7"
            }
          ]
        },
        {
          "id": "0999db92-a6fd-4f14-a11e-9752ab3a793a",
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
              "id": "16eedb1c-7f12-464d-9328-14ffe226ae01"
            }
          ]
        },
        {
          "id": "b3606abf-83a8-4266-ab8c-34a1e3537839",
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
              "id": "775edcb2-cf99-46e5-b3b2-302e4bc987c7"
            }
          ]
        },
        {
          "id": "a5546f51-08ac-477e-a180-ba616ad09b0f",
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
              "id": "438bfffe-40e1-45d7-af6a-5291031d3bbd"
            }
          ]
        },
        {
          "id": "2b3f04ec-0380-414d-807d-1c461d074781",
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
              "id": "d512c969-95d3-4f6a-8ea0-58a351ed2b85"
            }
          ]
        },
        {
          "id": "8b852871-eac3-4fb6-88fe-6873879f5984",
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
              "id": "3c9fd885-8c36-4482-b105-88a0001634b0"
            }
          ]
        },
        {
          "id": "835a3dc8-eea3-454f-8f51-43dd41635f19",
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
              "id": "bda11285-ecc7-41f7-8d1d-1d6a0480d1ec"
            }
          ]
        },
        {
          "id": "cb2923ff-42d1-41eb-be83-d4a398084e24",
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
              "id": "5443cda9-2605-4ca0-80e5-85adce44fbb4"
            }
          ]
        },
        {
          "id": "4a19418b-2729-4106-af6f-597a88906f7f",
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
              "id": "534b951d-4905-47d2-8559-e52927d37d06"
            }
          ]
        },
        {
          "id": "97dfd845-0b18-47a5-81b0-2e59780a03a4",
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
              "id": "05fa9105-a66d-49b8-8a7c-4be25338fd94"
            }
          ]
        },
        {
          "id": "67407482-ddcf-4107-8b1b-9291423d6ef6",
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
              "id": "1d31da52-4f5a-43b9-a330-3a426d0d97b4"
            }
          ]
        },
        {
          "id": "faf28098-68ca-4d4d-b7cf-f1487bae6871",
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
              "id": "54ad5702-8152-40ed-95d4-b0ab41c3c426"
            }
          ]
        },
        {
          "id": "27b7cb54-3d22-4e44-85e9-77d6d12b9d05",
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
              "id": "ed7cebdc-2f54-422f-9d26-3b923a7f8101"
            }
          ]
        },
        {
          "id": "5488c4fb-55f2-478d-aaab-5b040017da50",
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
              "id": "2d5125e8-2d1f-4b08-a212-324ffbd690c0"
            }
          ]
        },
        {
          "id": "8b885e04-2f8b-4cd4-96f6-67cbeb6b2532",
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
              "id": "c13969ff-f4f0-4c93-ab3d-014f24157164"
            }
          ]
        },
        {
          "id": "55e6e911-4086-4cc7-89a2-650ffd56b03a",
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
              "id": "39da5027-2824-4ab9-bab9-12c1fae4ab4f"
            }
          ]
        },
        {
          "id": "9dfd9e87-5c6d-4b77-8c73-1b56581fb83a",
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
              "id": "77980277-7730-4e6b-bb24-e0ba9dcc5ac2"
            }
          ]
        },
        {
          "id": "4f6f462b-aa7a-4aac-89e6-0d3437965cf0",
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
              "id": "75f359f8-168d-4966-a158-816b8294830e"
            }
          ]
        },
        {
          "id": "62ae62b9-2581-473e-a2f8-21007fdaa975",
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
              "id": "bac1ed65-9485-48b8-8002-03327aa5e783"
            }
          ]
        },
        {
          "id": "5705789e-c52c-40f8-86dd-4a66f62f0506",
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
              "id": "d2afb8ae-1291-4f75-a108-d7ef97124b17"
            }
          ]
        },
        {
          "id": "ebd650f4-e346-4f60-8d50-fb9358d02d1d",
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
              "id": "224f4a9b-53fe-4f00-96ef-bd90c48a5c6c"
            }
          ]
        },
        {
          "id": "fe3a030c-fc07-4337-9af5-8fd924b7acf1",
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
              "id": "800c1a9f-9485-4847-b5aa-06ac459fc386"
            }
          ]
        },
        {
          "id": "0c9802ee-9a9d-4d16-bdfb-b6ca6e5667a1",
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
              "id": "2a155642-5291-431f-8664-8776da7649ac"
            }
          ]
        },
        {
          "id": "82f8808b-584c-406a-93d9-b27cb8c7583a",
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
              "id": "bff76434-135a-4b0f-bce9-ed4ee571ad6a"
            }
          ]
        },
        {
          "id": "0ab70942-62bb-4d8f-a493-a82c6ad584dc",
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
              "id": "eb9ed5d6-68cc-476d-acab-ba3392ee455b"
            }
          ]
        },
        {
          "id": "afab2217-672f-4120-a6a4-99a58b015fbb",
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
              "id": "5f5e0e93-fa52-4af7-b284-075e064e550e"
            }
          ]
        },
        {
          "id": "75344317-7bc6-4ebb-b5a2-87097950fba5",
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
              "id": "762d7464-7caf-4af2-ab43-e55a67436cd1"
            }
          ]
        }
      ]
    }
  ]
}