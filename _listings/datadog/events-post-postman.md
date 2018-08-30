{
  "info": {
    "name": "DataDog API Add Events",
    "_postman_id": "be2f6e33-3878-45a3-8f40-885bb13bc8dc",
    "description": "Post an Event",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "2eb9ff9c-ab8b-4fe3-be76-caedba00fbb7",
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
              "id": "9254e741-0862-4e61-b047-10aa442269d9"
            }
          ]
        },
        {
          "id": "00640386-2d8a-451d-a866-ee379f4ea720",
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
              "id": "2168b0f4-de75-4f74-875c-a950982c8d06"
            }
          ]
        },
        {
          "id": "d0981994-aacf-44ff-ab70-713363fcb245",
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
              "id": "d9367f05-5e0e-4681-ac33-4db6fe007126"
            }
          ]
        },
        {
          "id": "f8a74fb1-e8a2-4d44-9f7f-f21ba7600513",
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
              "id": "6e8b426d-5e56-4ad7-991f-c8372e3723f1"
            }
          ]
        },
        {
          "id": "24029bc2-2785-4a23-81ed-d5c18b042864",
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
              "id": "ffcd68da-fb4c-4e2e-9afd-716843a3e046"
            }
          ]
        },
        {
          "id": "2faf91f6-856a-41d7-8042-e38114c32da8",
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
              "id": "d0619860-9355-4b53-b1b9-7791d45b26ed"
            }
          ]
        },
        {
          "id": "f2762d7b-4c75-4795-bbd9-11572b14588c",
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
              "id": "2536c6d5-0d1a-48bd-b4ee-13b1f91c40f8"
            }
          ]
        },
        {
          "id": "cd5912dc-22d7-4b25-bc1c-6ccfcbdcd842",
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
              "id": "e1790a67-4d4e-4537-a8cd-0b218b87aa1c"
            }
          ]
        },
        {
          "id": "e3d31c70-c955-4ad3-9f13-b5f6cce97c07",
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
              "id": "29a3652e-15f3-4043-8aca-801fcbf62320"
            }
          ]
        },
        {
          "id": "72658c69-43e0-4895-81e8-cdc7ff4dd89d",
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
              "id": "0b8c5e43-14f3-48f6-b85b-67afd821d0ef"
            }
          ]
        },
        {
          "id": "04c0f822-ac10-48ab-a1ba-9ca548e5c768",
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
              "id": "8c2507f8-1b8b-4cc3-895e-6be78266d98c"
            }
          ]
        },
        {
          "id": "748c5466-d6f3-42b0-aa4c-442151c44d5d",
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
              "id": "531ae7f3-0f5a-479c-942b-c4a13acf30c7"
            }
          ]
        },
        {
          "id": "4db4fa2e-bb44-4cb6-9913-398ab4ac71de",
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
              "id": "d5036f73-51bd-4593-b09f-d6064f1f71b9"
            }
          ]
        },
        {
          "id": "187c20d6-c546-4f68-a122-c19f1552a0b4",
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
              "id": "dae5f4b6-1a52-4fd7-9c08-cf4811080697"
            }
          ]
        },
        {
          "id": "bfd7d429-eac7-4087-9315-ef2eaa689f80",
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
              "id": "80d8c549-db63-453c-befb-40df7f2b350c"
            }
          ]
        },
        {
          "id": "a6dd78e2-fdc4-4432-bb10-cb83783417e5",
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
              "id": "69b48856-af37-41c5-a8ba-2e43a9d4db3b"
            }
          ]
        },
        {
          "id": "134ac101-767b-4bf5-8125-0f019336bf35",
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
              "id": "d84c1ad6-d947-486b-bcc9-67ae53532d66"
            }
          ]
        },
        {
          "id": "e2cea47a-07dd-4be7-85e7-f12baab5e295",
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
              "id": "1c20e4dc-1aaf-48a4-adbf-75ad6a52f0c2"
            }
          ]
        },
        {
          "id": "b3d1bb88-1175-44a6-a619-f9fa9edf1a27",
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
              "id": "7596d68e-7040-413d-8c94-9f7396b2872e"
            }
          ]
        },
        {
          "id": "74f06a5f-7a0f-475f-aa4d-ae39cc9b37ce",
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
              "id": "6ba0d88f-c838-4595-a7cd-775c3a521cd2"
            }
          ]
        },
        {
          "id": "934d1406-e3ca-40b9-8437-847583234c86",
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
              "id": "c4b5b6fc-4a50-49bf-b8f6-da29b7f804f7"
            }
          ]
        },
        {
          "id": "cd608db5-54b8-4351-a980-8d0453542a6c",
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
              "id": "669f996e-e4fc-48b1-aa84-65403a5d0bbc"
            }
          ]
        },
        {
          "id": "9f795086-9e9d-4005-aa65-f30b6000d94a",
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
              "id": "57e2bd6a-dc34-4e58-98cd-f01369cbe180"
            }
          ]
        },
        {
          "id": "dfeda6a7-dfce-4a22-9477-dd908fc0758a",
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
              "id": "22eb3a53-ed75-4fdb-a2df-081347bbef89"
            }
          ]
        },
        {
          "id": "78bd0218-4257-4416-8a5d-0cd066dfe8c5",
          "name": "getGraphSnapshot",
          "request": {
            "url": "http://example.com/api/v1/graph/snapshot?graph_def=graph_def",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET graph snapshot"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f22bfcd2-d913-4bc8-bf9d-d62d05f832e0"
            }
          ]
        },
        {
          "id": "7469c9bd-0c70-4013-acfa-dc00aad1e5fc",
          "name": "postEvents",
          "request": {
            "url": "http://example.com/api/v1/events",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post an Event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7901ef5e-2076-4b93-92a9-efa8f213ad1a"
            }
          ]
        }
      ]
    }
  ]
}