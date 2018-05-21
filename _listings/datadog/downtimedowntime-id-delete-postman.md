{
  "info": {
    "name": "DataDog API Delete Downtime Downtime",
    "_postman_id": "ced656fe-9155-403f-9888-c7e8b33835fa",
    "description": "DELETE downtime downtime",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "e0aeb501-5636-4007-8340-cd71977f5bec",
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
              "id": "332c4685-ca7c-4c82-8f3c-cbdbb1d0102e"
            }
          ]
        },
        {
          "id": "79462695-922f-4179-991f-92780a6c1bad",
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
              "id": "4f1015f4-a08a-4ba7-a7d0-7e8d4d0c4746"
            }
          ]
        },
        {
          "id": "392fab4b-27f6-40cb-aff1-22ff7dc9ceec",
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
              "id": "7d64192d-a314-4f70-bcc6-6ea510d4834d"
            }
          ]
        },
        {
          "id": "b4bf6a9f-6ac3-4ca1-8b31-9d214b048215",
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
              "id": "aed7f083-7dd6-4a68-90b8-792b35c1f064"
            }
          ]
        },
        {
          "id": "1d5c1f78-8ea5-4451-bff2-c26144cc099f",
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
              "id": "5ff2abde-0f2c-45eb-91e1-82486275736c"
            }
          ]
        },
        {
          "id": "04246956-67c2-46c7-8cf2-4561a377761a",
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
              "id": "852006e2-a070-4dcf-9d4c-5234ee97718f"
            }
          ]
        },
        {
          "id": "ab17285b-309b-4ab0-8ce3-16e961637b1c",
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
              "id": "df536e73-1b7a-45cb-abdb-fe0e44b76789"
            }
          ]
        }
      ]
    }
  ]
}