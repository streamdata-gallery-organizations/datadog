{
  "info": {
    "name": "DataDog API Get Screen Board",
    "_postman_id": "d43b6117-c11e-4ae6-8713-0568c63712e3",
    "description": "Fetch an existing screenboard's definition.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "40846c26-c5ac-4417-82f0-4aa099decf9d",
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
              "id": "5b022816-c775-4cee-988c-a106d5f6193a"
            }
          ]
        },
        {
          "id": "d35a5cf2-15e8-446a-a8f7-f9f1db8604fb",
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
              "id": "e8bbba96-22e8-446c-8b43-bdf1bfa7dc37"
            }
          ]
        },
        {
          "id": "00e50bb0-e72d-4220-92cc-52b02475d82f",
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
              "id": "8e30fd20-57b4-47b9-905f-40075280537a"
            }
          ]
        },
        {
          "id": "32165ad4-a6b2-4c81-a91a-01ad2963f58d",
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
              "id": "b174b6a3-88a9-4bb9-8734-a2ba5cdda253"
            }
          ]
        },
        {
          "id": "59dd0ac4-658c-4a1e-8b6e-e9efb631def5",
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
              "id": "7e884a64-d682-4d9b-a00c-e0bd1c52f5db"
            }
          ]
        },
        {
          "id": "c2472bf6-7fb1-41e3-877b-583348c50086",
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
              "id": "931d32bf-a97d-4f4e-b225-b9bfe56be79d"
            }
          ]
        },
        {
          "id": "dc43dff8-6b32-4d70-9935-bff8dc5b2e61",
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
              "id": "6bd404ca-6412-4aaf-8677-9e5433be3048"
            }
          ]
        },
        {
          "id": "90f34324-6fa1-4519-b2f1-62a8aca8d339",
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
              "id": "45da2745-66ee-4b42-8f26-fa9fd3159beb"
            }
          ]
        },
        {
          "id": "ffe2ddf0-e9c7-4549-9630-24a91cecd7c6",
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
              "id": "ff4c89c2-1cdc-4199-9d1d-4eb03a160114"
            }
          ]
        },
        {
          "id": "18df0e3b-6a77-4977-8f81-4c44cb41b215",
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
              "id": "b4e6d9b7-f8d1-404a-b23a-4ad3a9e4bc92"
            }
          ]
        },
        {
          "id": "7ab5d5e6-6053-46f9-85c9-e13140275359",
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
              "id": "5d91bc93-e44f-4403-bb5e-ef0487564366"
            }
          ]
        },
        {
          "id": "867658f7-4fb7-46c8-8f3f-b546da986cff",
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
              "id": "4db5642e-287a-4309-83a0-db155cb56acc"
            }
          ]
        },
        {
          "id": "fbc9c26b-61c6-43b6-b0a4-01d0a3940810",
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
              "id": "37c635a2-8f54-4dfe-933b-c508f6089c36"
            }
          ]
        }
      ]
    }
  ]
}