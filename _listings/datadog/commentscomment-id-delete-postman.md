{
  "info": {
    "name": "DataDog API Delete Comments Comment",
    "_postman_id": "2c77b4f6-784d-4e52-95d6-e351b354cf4a",
    "description": "DELETE comments comment",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "7f6d78a6-5c88-45d1-9c8c-24dfc4c5d5fc",
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
              "id": "6939d84e-c523-47fc-b880-12e323f0aba7"
            }
          ]
        },
        {
          "id": "3b84612a-25ec-4824-a3ef-0d417ad03f21",
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
              "id": "fc10e6a1-f999-4155-b371-f6127151eb4c"
            }
          ]
        },
        {
          "id": "6ecc2a5c-2c7a-4bb7-81af-42c787304e39",
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
              "id": "49a9ab9e-b0db-4ff3-986c-168f38f27686"
            }
          ]
        },
        {
          "id": "e78705fb-3eea-474d-9367-dcdcc614e04e",
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
              "id": "1c430dbc-3420-43dc-a2f1-e64c50676a1c"
            }
          ]
        },
        {
          "id": "dace0a57-58ce-4986-999b-25d53089b6be",
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
              "id": "faa9ac2b-7f51-4227-ab2b-4123c6841c23"
            }
          ]
        },
        {
          "id": "057e431a-4729-4574-b21c-a097e2fd4864",
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
              "id": "3dd4bed5-7c63-40d1-82d5-213909766a6f"
            }
          ]
        },
        {
          "id": "8bc76fbc-8956-4125-a346-2f99972c949d",
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
              "id": "42125a8f-6232-4f01-96e3-61d5767716b9"
            }
          ]
        },
        {
          "id": "73e3b6aa-5cde-4942-bc82-385839fae1a8",
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
              "id": "d25af65d-14b6-4e69-8ba8-c9fec7e73d6e"
            }
          ]
        },
        {
          "id": "4cf3b9f7-f81f-4f0e-8bee-eb5cbd77701d",
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
              "id": "a83f01bf-d8e8-467e-9c81-96ff1baba286"
            }
          ]
        },
        {
          "id": "9dbf802d-ec25-44b5-a899-79fea608cc7c",
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
              "id": "a47e29ec-4075-4a17-8683-d98023db6a1f"
            }
          ]
        },
        {
          "id": "6d1e5584-b3c8-4b40-992e-d43d583806dd",
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
              "id": "92a399f3-782b-47a5-a195-80b2c0f00a68"
            }
          ]
        },
        {
          "id": "19bbc93e-e406-490a-811a-ef994fdd2f34",
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
              "id": "64e8f2ed-91e2-4183-8698-81be98e5a797"
            }
          ]
        },
        {
          "id": "28d0565c-628b-4373-800d-d63634397785",
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
              "id": "4ba9ce82-894a-44d6-b0e0-e5b34e79b34d"
            }
          ]
        },
        {
          "id": "8684d358-a070-4d30-8aa2-6b690aa50d60",
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
              "id": "5d5bb81c-f4d0-4d2b-b099-4987d7c47798"
            }
          ]
        },
        {
          "id": "c29bd6f8-d8ad-46d5-acb5-3631a40d6bb7",
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
              "id": "83a44b0f-3dac-4fbd-a7bb-78ae69ff9bd7"
            }
          ]
        },
        {
          "id": "1af251cb-48ae-408b-9bf6-e2a16e7d3cba",
          "name": "deleteScreenShareBoard",
          "request": {
            "url": "http://example.com/api/v1/screen/share/:board_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Revoke a currently shared screenboard's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "592ac19f-1e56-442e-ac24-6406cf60f811"
            }
          ]
        },
        {
          "id": "6330758a-5596-4010-8b4e-60d4214ca797",
          "name": "getTagsHosts",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a mapping of tags to hosts for your whole infrastructure."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdc0b101-88a3-4113-8598-89fea81bbe94"
            }
          ]
        },
        {
          "id": "f494d5bc-bab1-41f7-bc3e-33885ad5c11f",
          "name": "getTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return the list of tags that apply to a given host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "087676db-b8ee-4b87-aea6-b36be743c867"
            }
          ]
        },
        {
          "id": "e85b5b24-b049-4856-b977-4c15adaafe78",
          "name": "putTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to update all tags for a given host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50bb97c3-3205-41e2-89fc-ed0d0c911e2f"
            }
          ]
        },
        {
          "id": "78639c5e-2143-4cf4-a0a7-79c80738cb52",
          "name": "postTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to add tags to a host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b11c3228-09ff-4057-b11e-55de051e176e"
            }
          ]
        },
        {
          "id": "6384ab70-6d88-46c1-831d-31077466b509",
          "name": "deleteTagsHostsHostName",
          "request": {
            "url": "http://example.com/api/v1/tags/hosts/:host_name",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to remove all tags for a given host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95869c41-a7b3-4233-8aea-2a6817b81a04"
            }
          ]
        },
        {
          "id": "d9616ce2-a519-4191-bb6f-a2f2a910d765",
          "name": "postComments",
          "request": {
            "url": "http://example.com/api/v1/comments",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Comments are essentially special forms of events that\n          appear in the stream. They can start a new discussion thread or\n          optionally, reply in another thread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba325040-08a5-4d27-9182-eb2526546261"
            }
          ]
        },
        {
          "id": "90fd4e95-3f29-4883-b8a0-c69f131cb2ca",
          "name": "putCommentsComment",
          "request": {
            "url": "http://example.com/api/v1/comments/:comment_id",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "PUT comments comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcf28e35-3854-4aef-933a-aba47a432449"
            }
          ]
        },
        {
          "id": "a6055902-d7c5-41a2-9f64-b7ba8d03e8df",
          "name": "deleteCommentsComment",
          "request": {
            "url": "http://example.com/api/v1/comments/:comment_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DELETE comments comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a9944ca-275d-47cd-8e12-2395e606668d"
            }
          ]
        }
      ]
    }
  ]
}