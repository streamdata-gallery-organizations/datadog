{
  "info": {
    "name": "DataDog API Get Monitor",
    "_postman_id": "5a9cbd3d-6a47-48aa-8feb-ff99ccd90724",
    "description": "Get all monitor details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "6295a0be-2f10-4ed8-a6c0-a8ad5a718b95",
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
              "id": "381e46f5-d8e9-4d36-8d8a-07286577805d"
            }
          ]
        },
        {
          "id": "16810bdf-131f-4981-9dd0-6213cc08214e",
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
              "id": "f1b42e0e-3ab9-4553-bc26-15ac61913728"
            }
          ]
        },
        {
          "id": "e068b6e6-3e6a-4641-bffc-2e9e1ca98732",
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
              "id": "0222f1f3-c564-4639-83e9-c706218c40db"
            }
          ]
        },
        {
          "id": "951dafff-c5f2-4bc1-984a-c295625382c8",
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
              "id": "32438ff1-ccb8-4bb3-b431-4c6c39057750"
            }
          ]
        },
        {
          "id": "3ff46699-2e2d-4b0a-95d6-8216a82f2779",
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
              "id": "dfd6b42f-3720-4112-b571-77770b38d0b3"
            }
          ]
        },
        {
          "id": "d307157d-4cdd-415a-94c0-998eb1cf6e45",
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
              "id": "ffe9635b-e3da-4458-bd8c-9a2c5b185357"
            }
          ]
        },
        {
          "id": "9375d57a-2146-4f6a-a1d5-dafb70d3c661",
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
              "id": "7d25b640-cedb-4bba-9e5d-967c80967850"
            }
          ]
        },
        {
          "id": "1a79d6d3-c21d-401c-bdff-24100b1c9e48",
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
              "id": "b8cce731-b115-4ed5-aeca-1fbaa8595c6a"
            }
          ]
        },
        {
          "id": "acb6a918-1fe8-41de-a332-6786ff807e71",
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
              "id": "ffaab265-83b1-46b7-b83d-a72b6f6fa307"
            }
          ]
        },
        {
          "id": "2af60919-3396-4e43-be1b-fcb131d6cb47",
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
              "id": "82ce54ed-4041-41ca-bcf8-f377a43cdf18"
            }
          ]
        },
        {
          "id": "47fa69f6-104f-4f91-9669-fdb37b22aa7c",
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
              "id": "d6d9adb7-169c-47d2-a6eb-553304f14875"
            }
          ]
        },
        {
          "id": "dab030af-be34-4e06-aa6e-9aa883efd40a",
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
              "id": "9944735d-1cf7-41b5-b466-1e9ea4fdf5b1"
            }
          ]
        },
        {
          "id": "4fff5f28-93c6-45d3-81f1-af36bea0473f",
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
              "id": "69dd7e4d-4442-44d3-9bc9-f728e6a2bdd0"
            }
          ]
        },
        {
          "id": "50259153-4495-4bc7-a727-4875decc6ca1",
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
              "id": "3d694ce8-b236-4587-aa8e-20d17f40269b"
            }
          ]
        },
        {
          "id": "a51755e3-37d3-47ec-bc70-9c6b86f392e2",
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
              "id": "17671c54-9717-4813-b084-ee13054e7c3e"
            }
          ]
        },
        {
          "id": "0640625f-8fc6-477b-abc0-8fdcc6524bde",
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
              "id": "c30fa2e3-95d1-4fbb-a8cb-5b9eebd6ff82"
            }
          ]
        },
        {
          "id": "e683cf11-e6a8-45cc-899b-22347165d2f1",
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
              "id": "298a8259-5926-48e9-9544-47349cd04e0b"
            }
          ]
        },
        {
          "id": "07f90f3b-e0bd-4a53-9d24-3af318080824",
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
              "id": "e936de31-bf13-4bcb-9e9d-23654af8d73b"
            }
          ]
        },
        {
          "id": "89a28e13-182e-4ba2-9905-64645adcac0f",
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
              "id": "eafc0a7a-4c80-4438-952a-ea9e17e515dc"
            }
          ]
        },
        {
          "id": "5d036846-ef28-4fb1-9458-3e1352fccd5b",
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
              "id": "dfa21928-8c74-4742-9bd6-44d744886e33"
            }
          ]
        },
        {
          "id": "9897e075-769e-4c87-9851-d50d34ed29ca",
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
              "id": "214b1e2c-a333-4885-8ed3-7ce38c66d710"
            }
          ]
        },
        {
          "id": "52e91234-c1e9-4b87-83c9-fbfe8e075494",
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
              "id": "20518ef6-6964-4c35-81bc-6bf34c34e8c8"
            }
          ]
        },
        {
          "id": "6acc1aa8-fe84-46ff-b439-6e172b970ff1",
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
              "id": "837ed851-11a2-4b25-9143-c26cad72a6a7"
            }
          ]
        },
        {
          "id": "b0d59367-90e1-4880-92dc-c9ea09491a8d",
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
              "id": "d6f93219-bef7-4c36-b455-fae362eced7e"
            }
          ]
        },
        {
          "id": "b85dcb34-28d3-44d3-adba-91c11b19c1b8",
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
              "id": "6f7381f9-2ab1-425e-a890-82ad073ad3e1"
            }
          ]
        },
        {
          "id": "b27f009a-9d0b-4a03-ad91-26ccc57e6375",
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
              "id": "7d10b7f5-457f-4403-9ee9-86604f54d1f5"
            }
          ]
        },
        {
          "id": "702f3c4e-5f2d-448e-816f-3b260795ce37",
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
              "id": "2c31b92d-fd17-41f7-bac8-6d45f5091616"
            }
          ]
        },
        {
          "id": "92bbd860-2b98-4ef3-883e-41e29c2df1e7",
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
              "id": "e01f6173-3c48-4bd2-bdd4-3a22439d4cac"
            }
          ]
        },
        {
          "id": "a77819b4-9007-406a-86a9-5a9e204a112e",
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
              "id": "d2861f1b-b267-4655-b19b-3e6a2363fb97"
            }
          ]
        },
        {
          "id": "70f729bb-e182-4316-b488-da6f7c604f35",
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
              "id": "88a531e5-09d2-4602-b947-bb0ae43997bf"
            }
          ]
        },
        {
          "id": "125b8321-5fd9-42af-899d-18a94341e55b",
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
              "id": "b6543212-1c32-4d6e-9d97-3a168901b1c9"
            }
          ]
        },
        {
          "id": "fa6e5080-2431-4654-ad0a-aa2994627e54",
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
              "id": "7181068f-7242-45b3-8470-2af699418f73"
            }
          ]
        },
        {
          "id": "f0461653-c0ba-4845-b8cc-2bef563427a9",
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
              "id": "c0c5ec05-cb38-4968-9267-ff6ae2a21f57"
            }
          ]
        }
      ]
    }
  ]
}