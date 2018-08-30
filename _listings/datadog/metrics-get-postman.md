{
  "info": {
    "name": "DataDog API Get Metrics",
    "_postman_id": "c213e632-a355-4f7f-92a9-31a9e8cfd998",
    "description": "Get the list of actively reporting metrics from a given time until now. This endpoint is not available in the Python and Ruby libraries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "5a6c882b-7536-4ca6-8ee3-41ac19e44d5a",
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
              "id": "5065639d-75a4-433e-acfc-f973dea0579a"
            }
          ]
        }
      ]
    }
  ]
}