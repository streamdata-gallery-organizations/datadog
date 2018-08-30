{
  "info": {
    "name": "DataDog API Delete Screen Board",
    "_postman_id": "a5b97746-4f8b-41d6-9f1f-a63a463fc3cb",
    "description": "Delete an existing screenboard.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "e5384881-8349-4f54-8299-8bcb4b53eecc",
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
              "id": "6ee45dca-a7e6-42e4-81b4-eb235967c195"
            }
          ]
        },
        {
          "id": "aa65c8e9-a0f2-47b1-bde3-6dc3f85d5a15",
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
              "id": "10d04db6-38a3-4e59-aac1-0fce477fdcbf"
            }
          ]
        },
        {
          "id": "20a40aeb-8c30-441a-a9a6-4b0f201f1886",
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
              "id": "c8746fd1-69f0-410a-8fe0-88798d1ae365"
            }
          ]
        },
        {
          "id": "232cb762-b2b3-49ab-907f-30d2e9d1204c",
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
              "id": "5dab594a-2a04-4fa5-b17f-0606c4a25a83"
            }
          ]
        },
        {
          "id": "eb2b70e9-0991-4dbf-a26c-04d5598729de",
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
              "id": "110841cd-5dcf-4d76-a4d8-a4b1952eaece"
            }
          ]
        },
        {
          "id": "293b8e95-4350-43de-af7a-c710b981becc",
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
              "id": "f894f9c4-a58a-4e19-9206-81e7757ca351"
            }
          ]
        },
        {
          "id": "36a6f916-a7a6-48ef-92ae-6e56b8d1ef0a",
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
              "id": "d658a44c-e8f1-462c-b100-1990f87f474d"
            }
          ]
        },
        {
          "id": "1b32f96f-8bd0-4313-a16e-8e4ecb7d04e3",
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
              "id": "27c4cbea-2f77-43d8-8ac2-96dcfdfe478a"
            }
          ]
        },
        {
          "id": "a159ad4b-68c6-45e2-aa51-edac6df3f5e5",
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
              "id": "e8139784-6374-48a6-ab05-0a58176d0df5"
            }
          ]
        },
        {
          "id": "da7a38fe-1b3b-4ace-b855-8a17ced8c668",
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
              "id": "5c069317-7b6f-4c01-8aed-874b0b282031"
            }
          ]
        },
        {
          "id": "4225e948-8209-4d5b-91f5-1d2dd58ded37",
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
              "id": "79905825-068b-45e4-9845-261a5cdcab6a"
            }
          ]
        },
        {
          "id": "58a3d521-5cc0-44a2-836f-262faba0a622",
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
              "id": "83969f80-1700-41e7-8df2-6abaeb4f3029"
            }
          ]
        }
      ]
    }
  ]
}