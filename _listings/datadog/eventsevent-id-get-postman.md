{
  "info": {
    "name": "DataDog API Get Events Event",
    "_postman_id": "44b4f150-a4c2-429a-981e-9d0cd35ca9bd",
    "description": "GET events event",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "40624e6d-72a4-4fcb-84c3-794fcaa6622e",
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
              "id": "cc56331a-8835-47f6-9cf4-c4335f8e5a3e"
            }
          ]
        },
        {
          "id": "0aa56251-8209-4a6c-b112-a0482cc7c475",
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
              "id": "b4ceb833-d59e-48ce-9ab4-b0587c21205a"
            }
          ]
        },
        {
          "id": "b607959c-c4df-4d4c-8020-9cfb490b2aae",
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
              "id": "a90023f8-4085-427d-987a-f1cd8a3886fe"
            }
          ]
        },
        {
          "id": "3d834146-d4c0-4858-a614-3a5d2f4295d6",
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
              "id": "8ec4d090-386e-428c-8d8f-bcc54028cdc6"
            }
          ]
        },
        {
          "id": "a4560e7e-0426-4a8e-9333-3362f40324c4",
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
              "id": "18a5eb71-a439-433d-ba75-5be9eba783fd"
            }
          ]
        },
        {
          "id": "41b2fdc6-1c03-4ca1-b18d-f2939719781f",
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
              "id": "7e4d1d97-72e1-4278-9f08-362723283176"
            }
          ]
        },
        {
          "id": "853703cc-f052-428b-b696-a8f0b59be283",
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
              "id": "d7fd3c7a-1d8b-42a3-ba50-c34d2ca633cf"
            }
          ]
        },
        {
          "id": "17c5b9fb-2a18-4258-abce-d5539266b0cb",
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
              "id": "93d42262-8b8d-4cfe-99a8-8e6fd968e80c"
            }
          ]
        },
        {
          "id": "dc5dbb9c-5d80-42d9-9a38-9ee2b00a3d93",
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
              "id": "7283e8e4-1b68-4861-8921-305139d18061"
            }
          ]
        },
        {
          "id": "b3815737-3cfc-46d2-a407-227a9d503cf1",
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
              "id": "a85cc483-86b9-4e78-b2ff-9d9d16f4e0d8"
            }
          ]
        },
        {
          "id": "440c6743-1c49-43ab-8671-b0e0519a732e",
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
              "id": "223d183d-5e86-4c24-af39-a826fb5d593e"
            }
          ]
        },
        {
          "id": "68b6d1c3-b3d4-4f7b-81c2-09a16d806244",
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
              "id": "98aa210e-14d7-4adc-85c8-97b9169ddccb"
            }
          ]
        },
        {
          "id": "2e1cbdad-93b9-48c0-abfa-00909deb409d",
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
              "id": "2add38e1-5e73-481a-abe1-1cbd6a6a7261"
            }
          ]
        },
        {
          "id": "f2ea9ebb-440c-4b16-8f87-1893591ecd4f",
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
              "id": "ff64ab1c-3d7c-4de1-a539-ef747b3058f4"
            }
          ]
        },
        {
          "id": "299d514a-cfc9-4ad8-913a-6c561fab57dc",
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
              "id": "4f8b57e4-3797-4312-96ec-3b6ad4f8dc57"
            }
          ]
        },
        {
          "id": "49b44629-6132-46a6-9962-79fe7e764e1b",
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
              "id": "f203fb34-9c50-4cd8-8af5-0123bcea4b03"
            }
          ]
        },
        {
          "id": "615ec043-3349-4ba2-9a13-f07b0c3796f5",
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
              "id": "de34f02a-ad69-4a4d-94b5-d594fb07da0d"
            }
          ]
        },
        {
          "id": "7d86a5ff-1141-49d4-b76d-593b0ff55d1f",
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
              "id": "c8f8c466-c5ca-4054-89ff-b5bab02d271a"
            }
          ]
        },
        {
          "id": "135095ec-2ac4-46ef-8416-10d1b424ff9c",
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
              "id": "0bd02cb2-831e-4c7d-9f38-95426c73ddf8"
            }
          ]
        },
        {
          "id": "561927d5-1215-4b9f-8849-a0910c5549f5",
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
              "id": "6e24db1b-c08a-4919-ac04-d4fea24cf26a"
            }
          ]
        },
        {
          "id": "f550021c-1ed3-4dad-a66a-5b489740517a",
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
              "id": "bb21d1c7-ae11-4a7c-9a50-0e23131b709f"
            }
          ]
        },
        {
          "id": "537d5308-73d1-457c-a84a-a0a6d55b6033",
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
              "id": "a58daa8b-91ef-416e-9f32-56372f66ddde"
            }
          ]
        },
        {
          "id": "c1c8eee9-7789-49bd-adff-fce66314fada",
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
              "id": "02176a76-b362-4e53-9101-1d4eec22c17d"
            }
          ]
        },
        {
          "id": "b65ca740-c84c-48b6-9af1-ef019cd7714d",
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
              "id": "8114d417-1a4e-453f-9eb4-776e05ded18b"
            }
          ]
        },
        {
          "id": "d6829b11-8a9e-450f-8dd2-ba7e542863dd",
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
              "id": "670fcb48-7fbc-4a75-a328-7abab59424c9"
            }
          ]
        },
        {
          "id": "f949e494-040e-415b-859a-3a7d788a50da",
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
              "id": "728e6bf8-fcc6-4026-8522-eed6e25e88cd"
            }
          ]
        },
        {
          "id": "24cfe2d1-5531-4fbb-abae-54526d332dd1",
          "name": "getEventsEvent",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GET events event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "532c4e2a-1fa0-41a8-96d0-a5f0bc1d7d4d"
            }
          ]
        }
      ]
    }
  ]
}