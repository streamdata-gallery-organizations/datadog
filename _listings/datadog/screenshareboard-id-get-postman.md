{
  "info": {
    "name": "DataDog API Get Screen Share Board",
    "_postman_id": "31968fa2-bbbc-4769-b831-9bfdcf16c5b1",
    "description": "Share an existing screenboard's with a public URL.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "54bc19bc-7879-4339-b4ba-cb20489fe73c",
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
              "id": "fd0cc5fb-acc7-4245-98a7-ec912377a83e"
            }
          ]
        },
        {
          "id": "15cb5aa5-91dd-4496-9d82-0c097cee5bba",
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
              "id": "7bcf61f5-7ee7-473a-b585-027f4c4bb0dc"
            }
          ]
        },
        {
          "id": "26f4374a-30f4-4b2c-b74a-d514f84a0931",
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
              "id": "95647517-4ac3-4826-b9dc-8d5370ba7dd8"
            }
          ]
        },
        {
          "id": "241e625d-8121-4fcc-a849-2a013c46e0b1",
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
              "id": "7bb738ab-457b-40ff-971c-51baa070b4f9"
            }
          ]
        },
        {
          "id": "e5ae937a-4160-4441-9e0a-6e9b61070f7a",
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
              "id": "41f2f019-59db-4d7c-9404-86a197242aad"
            }
          ]
        },
        {
          "id": "a1c1a2ee-c4b0-4e7f-b4e5-6e1172041d58",
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
              "id": "0575a760-e617-41b8-af55-9da6f3b547e7"
            }
          ]
        },
        {
          "id": "c904d8ce-f9a3-4f73-8b31-25624a612da3",
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
              "id": "016e8f1b-2760-43f7-a94e-529513fa76dd"
            }
          ]
        },
        {
          "id": "a0238281-249e-4ee7-ba16-fd9e10505bce",
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
              "id": "efc0468b-18c6-4f8a-9909-859806915134"
            }
          ]
        },
        {
          "id": "744db1ee-d735-4f74-b0af-08db5c964a73",
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
              "id": "4be84d95-f36d-4e7b-9c88-64408186bfe0"
            }
          ]
        },
        {
          "id": "49be8c63-6558-445d-b3d6-2ede1a7e1198",
          "name": "getScreen",
          "request": {
            "url": "http://example.com/api/v1/screen",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch all of your screenboards' definitions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05b7c4b2-2b4a-42e9-9143-84cc82f13e4c"
            }
          ]
        },
        {
          "id": "1b1c7d25-9598-4338-90c6-1d25fc1e4639",
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
              "id": "c3a68eaa-5ae1-4225-8a10-d5fb8b4c8c1e"
            }
          ]
        },
        {
          "id": "c806e53c-668a-404b-9e4a-1e6972b0f746",
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
              "id": "60c920a6-46aa-436a-b9f2-21bcaea70998"
            }
          ]
        },
        {
          "id": "697c92ec-f30d-409c-a98e-cbd7a3193111",
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
              "id": "c16cc4c7-2155-45c0-bf07-b7e11076b0c9"
            }
          ]
        },
        {
          "id": "a849a9ae-6561-402b-b3c8-6a72c475f4d0",
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
              "id": "f4bb9e2f-522d-444e-bc19-7321301f614d"
            }
          ]
        },
        {
          "id": "93dbfe8c-06fc-4077-b685-4a23eecc3be0",
          "name": "getScreenShareBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/share/:board_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Share an existing screenboard's with a public URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d88626a1-463a-4929-aaf8-ebb974c4b657"
            }
          ]
        }
      ]
    }
  ]
}