{
  "info": {
    "name": "DataDog API Get Screen",
    "_postman_id": "4cf1f5b6-ef69-4cb6-9b79-6adeaf24d65b",
    "description": "Fetch all of your screenboards' definitions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "7142a271-afe3-447c-8fba-4149e0ffcb9a",
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
              "id": "101bc3b2-75bc-45c6-85bd-344ae1c27266"
            }
          ]
        },
        {
          "id": "f07d228c-ee71-48c7-98c1-c868381ad1ef",
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
              "id": "1ac831ad-694e-4df2-9543-5dc3343510a3"
            }
          ]
        },
        {
          "id": "a9430e22-bf6e-451f-a617-40a95ff59765",
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
              "id": "425ce5d3-7c7c-4a4f-9c1d-f53d1b6b6e95"
            }
          ]
        },
        {
          "id": "45427dc1-465a-452b-bf19-b299a1dc6788",
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
              "id": "b9d65614-43d0-4804-98d7-a828cd83a809"
            }
          ]
        },
        {
          "id": "8089f6df-f153-4b53-b1e1-84294aff1273",
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
              "id": "49809ebd-156d-42af-88d0-9311382e84de"
            }
          ]
        },
        {
          "id": "af020021-0983-450a-90d8-650fcd165401",
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
              "id": "2d0a5cd0-6ad3-4891-bd23-c2f2a8aabe68"
            }
          ]
        },
        {
          "id": "7316b065-a37f-4abf-8abb-9f4a19326143",
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
              "id": "c53e4098-a227-41a1-9f85-2a40466df47a"
            }
          ]
        },
        {
          "id": "ed0c30cf-364c-4b78-873a-c62ae817f496",
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
              "id": "9f39f611-9ca7-4713-8aec-ea8af8377887"
            }
          ]
        },
        {
          "id": "837fbfdd-66aa-4c50-af87-beb91d7fad61",
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
              "id": "6c33d21c-0493-447e-925f-4de8bee1ecdd"
            }
          ]
        },
        {
          "id": "02ee945e-80f8-48d1-b0f0-4ecc77f52d3f",
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
              "id": "6c2f05ca-e084-49a6-9199-bed8b33a3bc1"
            }
          ]
        },
        {
          "id": "bac6c1c9-8182-41e5-a747-4a5915a6046d",
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
              "id": "11d0c591-b63b-4d3d-8951-0ac1d70ac20e"
            }
          ]
        },
        {
          "id": "000217c5-cf10-4cc0-8a5c-ba24d5ef9cfa",
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
              "id": "47e84d02-9026-4008-b048-2f16754c2750"
            }
          ]
        },
        {
          "id": "9656d367-f51a-4a14-bcd3-a9b02cf41f04",
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
              "id": "255da00d-8dac-4646-905d-a0e58afa6119"
            }
          ]
        },
        {
          "id": "64a3417f-508a-4a70-b5be-0dc64d7ec6ab",
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
              "id": "5e146ef6-f981-418e-a172-60d989cfcb0f"
            }
          ]
        }
      ]
    }
  ]
}