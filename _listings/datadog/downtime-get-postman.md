{
  "info": {
    "name": "DataDog API Get Downtime",
    "_postman_id": "bf6b6144-91c4-4e3c-bfe5-3ebdfeabb799",
    "description": "Get all monitor downtimes",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "6bf50b23-b997-4534-adef-af42fb39e4fd",
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
              "id": "77424f16-7cb8-4751-9995-03f3b4f4ca3f"
            }
          ]
        },
        {
          "id": "f7da785c-7658-46be-a8a0-d9003733de30",
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
              "id": "553b9dc6-d3e4-491a-b0d7-eea597d45fdc"
            }
          ]
        },
        {
          "id": "3f1a8413-ed0e-41a5-801f-a6f130f88f4a",
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
              "id": "6e3b16e8-334c-4198-b6ca-c01af058da74"
            }
          ]
        },
        {
          "id": "8c447bfb-1d75-4f78-8f49-99de86cf2e7e",
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
              "id": "86f7b3a4-f44a-4984-95c4-80a92794e3ce"
            }
          ]
        },
        {
          "id": "3a418954-f47b-47a5-b197-ad35681ddafc",
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
              "id": "98c78e80-bdd1-47f5-9527-9766cb9c66dc"
            }
          ]
        },
        {
          "id": "69e4e0a6-2a2e-48a5-83a9-6058821f416b",
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
              "id": "2c4ad447-aa37-42fd-a4e9-46d148b61af0"
            }
          ]
        },
        {
          "id": "29bc026d-6bf1-4cb5-bbe6-0d945060b46a",
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
              "id": "5efce2e8-bb23-4e1f-be2a-11685db78d99"
            }
          ]
        },
        {
          "id": "d5813144-03db-4f38-8198-cdf73cf64b44",
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
              "id": "aa6de23a-b4ca-43c8-97f1-7c557336472d"
            }
          ]
        },
        {
          "id": "e4e110de-5de8-4fec-b3f9-c0422e757ab2",
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
              "id": "81d46775-086a-42c2-8d76-816ba9ab7264"
            }
          ]
        }
      ]
    }
  ]
}