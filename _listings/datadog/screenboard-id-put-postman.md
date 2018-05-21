{
  "info": {
    "name": "DataDog API Put Screen Board",
    "_postman_id": "e0f80c7a-15f3-479c-b8ae-a7222515ff9b",
    "description": "PUT screen board",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "e9c4ab19-2249-4849-ba64-2d33ec820f05",
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
              "id": "c42e8a89-8c6d-4653-96da-3d03aa157b5e"
            }
          ]
        },
        {
          "id": "de6adc12-c112-41eb-ab44-7666e43d60ec",
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
              "id": "251f2428-72c9-4d04-8124-f7d3e6d71c86"
            }
          ]
        },
        {
          "id": "95e1307e-4773-4d28-83a5-8cc50a09cf5c",
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
              "id": "a84f25fd-b8d6-4194-93f5-99d38bf09c7c"
            }
          ]
        },
        {
          "id": "22ce0746-a4d6-4016-91d0-a82928db6a59",
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
              "id": "20818e21-9bd4-4985-a5f4-876346ce62ec"
            }
          ]
        },
        {
          "id": "b7f02cdc-5dd2-45c3-b746-4a7271a86d6f",
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
              "id": "520e2d21-3168-4a0e-b433-6d4bc404cc4c"
            }
          ]
        },
        {
          "id": "cbcc1654-88bf-492e-9ba6-1d49915cbda0",
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
              "id": "f0299a23-a1fb-4ed5-8a3f-af062e99a062"
            }
          ]
        },
        {
          "id": "3fe27a85-0bfe-4332-a8f2-bf8df27b82ae",
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
              "id": "8870d033-2c3a-4295-8bc8-75ac7c2bfeec"
            }
          ]
        },
        {
          "id": "bc0e65c7-2ec8-4fd2-883c-0306cdb3c3bd",
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
              "id": "b3bf517e-0681-4349-8036-ff230b2fd1a9"
            }
          ]
        },
        {
          "id": "e174930a-990b-41a8-addb-4699909aa901",
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
              "id": "fe8d76ba-9dcc-4e5d-9069-38424aa5cb0d"
            }
          ]
        },
        {
          "id": "6bd8463f-16a0-45a0-a0c1-abd613390f90",
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
              "id": "6e70f682-2499-480e-a857-a30a7ecaabe3"
            }
          ]
        },
        {
          "id": "9e013436-9b45-47a3-8f56-a86e483d248c",
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
              "id": "84a29eee-4690-47d7-bc40-93873c179878"
            }
          ]
        }
      ]
    }
  ]
}