{
  "info": {
    "name": "DataDog API Get Query",
    "_postman_id": "2e399ef4-21be-45ff-8adc-e3e00519c26d",
    "description": "This end point allows you to query for metrics from any time period.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "079ebb10-3f6e-47a1-aa7a-5ed1faca02fc",
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
              "id": "cb6f5603-123a-4001-a6ef-b407ddc710c9"
            }
          ]
        },
        {
          "id": "086b019c-0e6f-4e94-b912-88a8a33052cf",
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
              "id": "218c1296-3675-47b8-9d25-1ccae7315193"
            }
          ]
        },
        {
          "id": "bb9a2945-90b2-432f-aacb-8dd68d0dbe44",
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
              "id": "26b229f5-1b50-47b6-b737-cc57396093d8"
            }
          ]
        }
      ]
    }
  ]
}