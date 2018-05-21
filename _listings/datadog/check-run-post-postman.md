{
  "info": {
    "name": "DataDog API Add Check Run",
    "_postman_id": "a7405611-87c9-49bc-84d7-aa414ad5b6c5",
    "description": "Post a Check Run",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "e1fbda01-d6b6-4f35-978b-6f77e2e60d51",
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
              "id": "59c3f05c-379f-4b4c-bb4f-5a246d51b4bf"
            }
          ]
        },
        {
          "id": "21b23840-3fc7-4ed0-b601-f2654437e600",
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
              "id": "0df6ad30-b71d-44ee-8a77-3ee1a712f3a6"
            }
          ]
        },
        {
          "id": "25fda258-64c3-4f97-9cb3-e6701afdc769",
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
              "id": "51e35f7a-dca8-4fe2-98b9-d4a518aa748a"
            }
          ]
        },
        {
          "id": "cd5cb61f-de1c-4beb-b178-5e9d7173f95a",
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
              "id": "d0c98a62-3913-46b0-8127-adad91de3643"
            }
          ]
        }
      ]
    }
  ]
}