{
  "info": {
    "name": "DataDog API Add Screen",
    "_postman_id": "484ed958-9320-4e24-8cd8-869befc2f5db",
    "description": "POST screen",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "e3e40973-936a-40f5-ab6a-f852a1f4fbfb",
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
              "id": "7c3d93a1-68e0-4f19-99b3-bf488c6ccb60"
            }
          ]
        },
        {
          "id": "af67846b-16c5-4a6a-b049-4ec3653fee77",
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
              "id": "5b5d8197-5f05-4911-a37f-8ead558991ae"
            }
          ]
        },
        {
          "id": "64eccee8-e424-4bc7-995d-a73a9bcfe967",
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
              "id": "d48f19e8-aa62-4b36-a491-8faa36e5bc3d"
            }
          ]
        },
        {
          "id": "abd348f2-746d-40af-97c5-9d8c9b382172",
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
              "id": "c092226b-ca87-49eb-82ab-773330d430e7"
            }
          ]
        },
        {
          "id": "c4abf070-376a-4933-8713-7924d9e13745",
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
              "id": "6bb51ae6-b1e3-43d0-ac67-bb6b964d9ed4"
            }
          ]
        },
        {
          "id": "883bfe34-39b8-419e-b30a-a9623704e8c6",
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
              "id": "f96e55ae-1430-4f5c-9742-3662b1e523e8"
            }
          ]
        },
        {
          "id": "2e8196aa-08e9-4ebf-a450-8a6afa0d9cfe",
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
              "id": "d80f09a8-fe45-414e-becf-fcdb7a2dae3e"
            }
          ]
        },
        {
          "id": "07e2f71b-17a2-4c46-845f-760a38229d2b",
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
              "id": "b365e87b-6ba4-4750-89a0-e30b6d005d11"
            }
          ]
        },
        {
          "id": "1528e60c-60fa-45bc-bb19-ab8d9903de3c",
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
              "id": "24eb89a9-5237-4a02-b47f-fa0fe2e5fbc9"
            }
          ]
        },
        {
          "id": "65bfb492-941a-4c56-8a28-a9812ffee7f4",
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
              "id": "fe61162a-11e2-4562-8e22-c7d3f1a24262"
            }
          ]
        }
      ]
    }
  ]
}