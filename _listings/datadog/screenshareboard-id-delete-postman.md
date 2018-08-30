{
  "info": {
    "name": "DataDog API Delete Screen Share Board",
    "_postman_id": "042027c8-bcbe-49d7-bfa0-f37300ab5603",
    "description": "Revoke a currently shared screenboard's.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "2c21cfdb-2c53-49ec-89a3-b82309b28659",
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
              "id": "1e95905e-829f-4d5e-b4aa-8f9b79cb6c99"
            }
          ]
        },
        {
          "id": "cc9f8887-afff-427b-a15d-d9a6025292ee",
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
              "id": "c102df30-502b-4eda-9705-877ec7abaaa3"
            }
          ]
        },
        {
          "id": "1ae72b60-87dd-431a-8fb0-a88def611045",
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
              "id": "2b07e970-8ec0-4461-a750-ee64aff99301"
            }
          ]
        },
        {
          "id": "0b49c189-387f-4218-b504-8542b4547aa5",
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
              "id": "1e10076d-0ec1-4810-9180-fbaf2854ee3c"
            }
          ]
        },
        {
          "id": "c52931e7-1ad4-4b38-b95a-002385b2e4c2",
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
              "id": "0d16e167-e468-40a6-8590-9dc8bda8e339"
            }
          ]
        },
        {
          "id": "1c69153e-fc27-479b-82de-37f7d025228a",
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
              "id": "a1977236-5398-4784-8d24-ead975c6d708"
            }
          ]
        },
        {
          "id": "054ab9b5-d3e8-4a32-85a4-e93e35b8d4a0",
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
              "id": "9463dda4-1fc4-43fe-8536-c04f7cd07017"
            }
          ]
        },
        {
          "id": "b138092d-fb1b-45ef-ad04-ba36f5436370",
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
              "id": "d5a3fa2d-56d2-4208-8126-53e9a9078f90"
            }
          ]
        },
        {
          "id": "405840ee-3d2c-45c9-a401-d8ad582e6beb",
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
              "id": "fa2863ea-aeb8-47c9-a6c0-8c13100726c7"
            }
          ]
        },
        {
          "id": "2781e657-d3c7-41d7-9d2e-b41267f11f8f",
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
              "id": "29fd189a-c470-431d-bafb-15cf8402bf3b"
            }
          ]
        },
        {
          "id": "20069b1f-8f43-427e-9b7b-faa43bf2aeee",
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
              "id": "d7faccb0-0d09-4e83-b34d-111f7d77b0a4"
            }
          ]
        },
        {
          "id": "cc9980de-1680-4a90-a20b-3ac6bec0eea1",
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
              "id": "cf410398-0bab-4774-aa34-6b0b7f16c381"
            }
          ]
        },
        {
          "id": "175fe50e-335f-4ebe-bef1-cfdc460f367c",
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
              "id": "9fbafefc-9548-49cd-8b0e-17d6b504e5b3"
            }
          ]
        },
        {
          "id": "72c9a276-08cc-481f-960e-e162f35156f8",
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
              "id": "41075c52-817d-4bb4-ba65-4534d52f63bd"
            }
          ]
        },
        {
          "id": "32ef93d6-2be3-4b02-be59-a65ec21edde1",
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
              "id": "15cb84a4-cfc3-4ca7-a42e-53a348ab7db5"
            }
          ]
        },
        {
          "id": "84dc67e4-7ea3-4f43-a941-0b10c64fa9d8",
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
              "id": "7756824a-d32a-419b-b22d-3d58ee7a9453"
            }
          ]
        }
      ]
    }
  ]
}