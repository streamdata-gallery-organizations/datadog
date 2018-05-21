{
  "info": {
    "name": "DataDog API Get Downtime Downtime",
    "_postman_id": "81a711bb-63ae-42c1-806f-81a627134ad0",
    "description": "Get a monitor downtime",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "511c3e88-34bf-4c3a-ab3a-0dd5b776483a",
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
              "id": "68fe5291-d797-4a5f-baa8-f2a5206c1cc6"
            }
          ]
        },
        {
          "id": "ad64110f-58b2-4e8f-9cd4-c729ac4abec5",
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
              "id": "b29a3bea-ed0d-4ece-9169-9c21a22693ca"
            }
          ]
        },
        {
          "id": "1de811fe-d1bf-4f91-ac89-35b98afade4a",
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
              "id": "06856fb0-a1b0-46b0-80c6-be3529dc76a9"
            }
          ]
        },
        {
          "id": "379d96de-d9c4-49a2-b6b0-9d31bd51c5bf",
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
              "id": "07eb6e1a-9383-4279-83c8-3944f0e8ae23"
            }
          ]
        },
        {
          "id": "61456d88-b2e6-4ab1-a41d-b52a76788770",
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
              "id": "b7d06a14-0f45-45a6-890c-fa98bcdf3a5f"
            }
          ]
        },
        {
          "id": "3624f75b-4fe4-4d3c-9648-5eb566a7f79d",
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
              "id": "53468b30-fddb-43ea-aed8-341d97085e53"
            }
          ]
        },
        {
          "id": "91c9cbad-0ce6-40b0-93cd-311dcc49f4ce",
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
              "id": "73655cbd-d859-4f52-b29b-061d5439126d"
            }
          ]
        },
        {
          "id": "aa07e1a1-0527-4d99-9012-b1aa91dc0611",
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
              "id": "fa1dfb55-4845-43c6-8f4d-075a9a504aef"
            }
          ]
        }
      ]
    }
  ]
}