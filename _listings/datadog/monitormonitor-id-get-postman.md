{
  "info": {
    "name": "DataDog API Get Monitor Monitor",
    "_postman_id": "b2079e1d-b9e7-41e1-81af-574ff28c3cca",
    "description": "GET monitor monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "ccf8800a-4747-48d4-9624-454b131342cf",
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
              "id": "7da1f17d-9bc5-4c82-86c5-eca0eabd1006"
            }
          ]
        },
        {
          "id": "76a57564-7772-4dc7-84b5-606210c09004",
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
              "id": "1f851adc-0525-479e-81cd-42cc9eedb808"
            }
          ]
        },
        {
          "id": "f2f06882-9940-4c49-9483-9d81ee0a9ce1",
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
              "id": "f10d6d91-d5b7-4117-8778-05c7b5b58ddc"
            }
          ]
        },
        {
          "id": "e88ce64f-343a-4782-8db1-ac3732d40327",
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
              "id": "8f932023-d451-437a-a88b-0fe2480c1e33"
            }
          ]
        },
        {
          "id": "87bc5ee7-32fb-4637-b589-480ec339e80e",
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
              "id": "547f2ecc-57dc-45bc-a112-7cd340140a06"
            }
          ]
        },
        {
          "id": "ef17594d-7b42-4161-97bf-fa3f8ebdf728",
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
              "id": "a20a4a3d-a4cd-4e2a-bb6a-17e2774e86b3"
            }
          ]
        },
        {
          "id": "a0421e39-b0fb-4dcf-98ed-3096e64962a5",
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
              "id": "e4e9632f-b1cf-4230-9faa-0491927210e2"
            }
          ]
        },
        {
          "id": "d08bc528-018a-4b66-a5c4-6f4fb8a5fe4b",
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
              "id": "f7eefb97-0147-414d-b441-9be9afd0b3ae"
            }
          ]
        },
        {
          "id": "22628614-d54e-4a70-ba43-034656161124",
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
              "id": "c1d679e7-02d5-48b9-addf-2808d1140d1d"
            }
          ]
        },
        {
          "id": "5454e9ce-e271-46a6-b016-f86cec29a116",
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
              "id": "99c7ecfe-fc33-4930-a52e-2813c623fcec"
            }
          ]
        },
        {
          "id": "ee91c086-c474-4da5-b163-b89660268e5d",
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
              "id": "d8175943-6194-41f0-a70e-e39600e233fc"
            }
          ]
        },
        {
          "id": "de354393-f47c-4b7c-bac8-3ffe655e1a8c",
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
              "id": "38afdefd-002f-4d59-975f-9106942397dc"
            }
          ]
        },
        {
          "id": "2f1896bf-e645-4db9-b179-8a26a4fd22d4",
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
              "id": "362bc01d-6c97-4752-bb73-a6453a3ce274"
            }
          ]
        },
        {
          "id": "e330103b-e0a9-47e3-bcf7-19671269cf62",
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
              "id": "f65c9a2c-e83d-4755-91f4-da2cb2a8ea23"
            }
          ]
        },
        {
          "id": "02aca905-dd2b-4508-9e6e-41f26403d919",
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
              "id": "7ce31e89-a6fb-4eae-82ba-8a97bc12e8b4"
            }
          ]
        },
        {
          "id": "3553765e-ea2e-47e2-8b8b-2f1e4de1c320",
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
              "id": "540cab03-923e-4590-995b-5be6248a44af"
            }
          ]
        },
        {
          "id": "00cc40ae-b002-4421-bc82-e27c53641ee8",
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
              "id": "954b9436-32ef-4b4b-a60d-6fedad871d08"
            }
          ]
        },
        {
          "id": "841009a6-376f-4736-8417-e61cbbc34df5",
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
              "id": "3b2dd865-1d1b-4f4f-b991-8e14040db660"
            }
          ]
        },
        {
          "id": "e1780d11-ee20-4201-8b28-ea9698f14fd4",
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
              "id": "d7686ec3-6709-42bb-ad37-fcd3b9373683"
            }
          ]
        },
        {
          "id": "c6f84d6d-1aa3-44d7-9eb2-95bb149b152a",
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
              "id": "a5ee06e0-cbbc-49e1-9e50-37d0e16d1d58"
            }
          ]
        },
        {
          "id": "8322ad4e-3eb1-49a4-b686-50829381b29c",
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
              "id": "1f8bc959-e506-4c23-9859-a320023addbc"
            }
          ]
        },
        {
          "id": "759b9465-de1a-4a04-a70e-806e36da192b",
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
              "id": "c31eff36-38bd-4781-8c40-a2cf9d34b178"
            }
          ]
        },
        {
          "id": "1ec609d8-0977-46e0-8b75-f51ca7836864",
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
              "id": "a5a1de15-59bf-441d-8b8c-36e5353037ce"
            }
          ]
        },
        {
          "id": "cf104b9c-226c-4c2f-933d-3daeb510860f",
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
              "id": "75978697-22f7-4972-831c-cf5eea1085bd"
            }
          ]
        },
        {
          "id": "d92874aa-35a3-4929-a3d2-b9bea84664bc",
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
              "id": "a1c5ffed-3300-4506-8bca-65e4e66ec9f4"
            }
          ]
        },
        {
          "id": "3779507a-f55a-4d78-bca9-8a9f0902b59b",
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
              "id": "7ec2a08c-c69e-49d9-9ed4-7ac98f0ffdc7"
            }
          ]
        },
        {
          "id": "e4098edd-a1e5-4b94-b87c-2baac0b6a98a",
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
              "id": "0568f9ac-1c5c-4795-a1b8-9e0bf0d5f4b7"
            }
          ]
        },
        {
          "id": "b479edcb-48ed-47d3-b61e-b330be408b4e",
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
              "id": "37dfcd66-b46d-4228-a273-615dfb73604d"
            }
          ]
        },
        {
          "id": "da431355-e83a-4302-88e0-8bed81b7008e",
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
              "id": "4f633e1b-cd55-4e33-96ce-f031463beb10"
            }
          ]
        },
        {
          "id": "eed22f93-2aa3-4d59-844b-510cc3f158a7",
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
              "id": "2a17caaf-bcfb-4b07-bfe6-57ea0fdbbfe7"
            }
          ]
        }
      ]
    }
  ]
}