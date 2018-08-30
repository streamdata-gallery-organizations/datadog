{
  "info": {
    "name": "DataDog API Put Comments Comment",
    "_postman_id": "2e99a339-734f-4e04-8ae9-18fe517cbc35",
    "description": "PUT comments comment",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "1a392e44-de09-4539-bf1f-562debc1ddfe",
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
              "id": "0c5b5e5a-ec65-44e6-8ce0-d502c454565a"
            }
          ]
        },
        {
          "id": "02443893-4a05-4003-9384-66242faba596",
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
              "id": "8c977963-f1e9-46fd-88cc-ae9306f3fbfb"
            }
          ]
        },
        {
          "id": "55c4c055-e36f-4432-af6f-d61462464a0b",
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
              "id": "4d516f45-95ac-4aa0-9b58-863781357234"
            }
          ]
        },
        {
          "id": "0feb9444-8b7d-4ae8-bd53-cd5580dbb99a",
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
              "id": "42eda5fb-9248-4555-a0de-f94e6e06c55d"
            }
          ]
        },
        {
          "id": "880189b9-ceb4-4008-a51d-b81211b66ee0",
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
              "id": "758883d9-b354-44d7-9c4f-b397a7d632ac"
            }
          ]
        },
        {
          "id": "5d29b6f0-b12f-4b97-81f2-f16dc3434209",
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
              "id": "638add5b-bbab-48ed-9bc7-a3d40276657c"
            }
          ]
        },
        {
          "id": "e32a0aef-03cb-40dc-9cba-4f901647f62a",
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
              "id": "51eb5dcd-e522-4e50-9795-5971caf28fba"
            }
          ]
        },
        {
          "id": "0d782cd6-1ca4-40e0-a083-0adc25182a7f",
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
              "id": "f333252e-5565-4e37-9dc6-c4043deb1017"
            }
          ]
        },
        {
          "id": "a95ef1c0-5614-4726-a81b-d5db091afd53",
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
              "id": "a4c80179-958f-45aa-9e79-4a281debaa7d"
            }
          ]
        },
        {
          "id": "27576ff5-2dc4-4846-936f-f1d048fe0d14",
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
              "id": "24499e60-7348-476f-a0fb-27cc7f544442"
            }
          ]
        },
        {
          "id": "3b2d2de7-8e0d-4d79-b4ba-f318d0d6db42",
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
              "id": "313fb1c4-e220-4081-8e42-173735c60633"
            }
          ]
        },
        {
          "id": "157a3a77-674f-480c-bda5-db2777d8e7b7",
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
              "id": "e1e5e398-670c-42a6-91b5-1b4a1fbdebac"
            }
          ]
        },
        {
          "id": "e454b7e0-2ea8-4983-a7e9-32c755e74cea",
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
              "id": "3ac6915f-b997-466f-adbe-ae34c645aab0"
            }
          ]
        },
        {
          "id": "362538cc-1b3a-4849-b0de-fefe8b4667fb",
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
              "id": "26c8f88b-7f6c-445b-9edc-8ea16a1cf321"
            }
          ]
        },
        {
          "id": "d73bf3d0-c66c-476f-a98e-dfc12fd89a95",
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
              "id": "ab5bb824-5e02-4bb6-82a3-b6e2ab7f73c4"
            }
          ]
        },
        {
          "id": "0db1af8c-453e-4bbe-bafe-a3d2a77d98c1",
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
              "id": "7f2c2204-811a-450c-864b-e091014a2638"
            }
          ]
        },
        {
          "id": "be4296df-95ca-477d-83ea-814f9692f11c",
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
              "id": "8356a692-eece-427c-9927-3ab3e2962337"
            }
          ]
        },
        {
          "id": "6e76a0a0-7c63-44d3-8be6-865571781678",
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
              "id": "df8e73a6-3814-4d18-a1c5-6833cde0c9e2"
            }
          ]
        },
        {
          "id": "7119ccc6-b4c7-4ea8-84da-a4a4ae1b89ff",
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
              "id": "0d792569-82f5-4bea-9298-86c33d8a6dfc"
            }
          ]
        },
        {
          "id": "b76e4ca2-2733-4824-adb7-26311c2fdead",
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
              "id": "80c7e2fb-6399-470c-8128-951290c5bdf5"
            }
          ]
        },
        {
          "id": "2303a064-2dd4-4081-8f03-ab89fc9a5850",
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
              "id": "41e228d6-9d9f-43d8-afa2-ff0900f21e63"
            }
          ]
        },
        {
          "id": "69e60215-149e-46da-97b0-073a4a7265cf",
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
              "id": "00594a3d-9364-4762-9079-18d2137d184e"
            }
          ]
        },
        {
          "id": "e9ba24a7-a725-4310-b30e-b36188370453",
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
              "id": "af40f48e-f4ed-42f6-a7db-02d330e54b93"
            }
          ]
        }
      ]
    }
  ]
}