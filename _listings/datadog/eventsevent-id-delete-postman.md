{
  "info": {
    "name": "DataDog API Delete Events Event",
    "_postman_id": "669398b9-bd45-4bc2-b358-15159afb0b2c",
    "description": "DELETE events event",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "111b2de7-db2c-45d5-b81b-4717fd936a25",
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
              "id": "6ab0f8e0-8705-40a6-9030-2788138e7d36"
            }
          ]
        },
        {
          "id": "00d3a119-372b-4feb-a4ef-7081933af3fe",
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
              "id": "1483866b-b94d-459a-a288-fef4b3bf9624"
            }
          ]
        },
        {
          "id": "4a060a1c-3526-4f47-aec0-cfd0cb2f9ca4",
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
              "id": "eab81649-0134-494b-be37-4bd71c5e5fd1"
            }
          ]
        },
        {
          "id": "e85ce890-8593-4cd7-b94f-b7a3484fe7fc",
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
              "id": "d8f81233-b41e-49ff-bb9c-1548192b8133"
            }
          ]
        },
        {
          "id": "b2896cb0-e80b-40d9-8d0f-c4d86b035cf6",
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
              "id": "0a36280f-20bd-4de0-aff0-d6f2bb63ec4a"
            }
          ]
        },
        {
          "id": "b88db01e-6632-4b81-a03c-34ff4cc31d28",
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
              "id": "a0aa0e20-7ca8-4f2d-9fb8-14e89c2c0653"
            }
          ]
        },
        {
          "id": "461509b7-a678-482d-b4c1-fab28feca4e5",
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
              "id": "24d0a2d0-e6b4-4781-95ef-ac25fa6f0378"
            }
          ]
        },
        {
          "id": "9a4c4681-9da3-41f2-ace9-c6953dfb7102",
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
              "id": "c495ba8c-0ec9-44cd-9fed-567f6a839513"
            }
          ]
        },
        {
          "id": "cd5e1fa8-fc20-4b5f-90a2-6742484e41c9",
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
              "id": "c466a3cf-1725-4bf8-a068-33b6dee99b18"
            }
          ]
        },
        {
          "id": "e027d145-cc7c-4311-93ca-7a2a051974a3",
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
              "id": "90587408-2435-46e7-a502-d43f0f0a2cdc"
            }
          ]
        },
        {
          "id": "45138cdc-66e7-46f3-9953-ac270c8fb904",
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
              "id": "243bd175-a5a6-41df-9f76-58cb566ff6be"
            }
          ]
        },
        {
          "id": "741178f6-fe8c-477c-9fe7-885386d0f8df",
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
              "id": "5576d73d-42f8-4f40-acb1-54f8e0c79dcc"
            }
          ]
        },
        {
          "id": "4649bee8-77cb-486e-9436-efc1c7993060",
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
              "id": "fc68f24c-d27d-47c8-819c-bc6c85e4776f"
            }
          ]
        },
        {
          "id": "8101ac25-74e6-445e-af7b-99f54d0c5021",
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
              "id": "33697e8a-fac9-484a-8a39-c6ad88f708f5"
            }
          ]
        },
        {
          "id": "337fcaac-2166-4989-87d4-ea1c2c519c86",
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
              "id": "f4e9c3ad-3f21-4d53-9b30-ab5af58b73d4"
            }
          ]
        },
        {
          "id": "181d599a-6f00-4483-9a13-67243eb77933",
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
              "id": "e3865652-2563-4578-8544-b3c6fc33ab09"
            }
          ]
        },
        {
          "id": "02061e67-0768-4907-a8ad-6f0d1dfd4b5c",
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
              "id": "89701074-1a1d-4d61-88de-471af068687d"
            }
          ]
        },
        {
          "id": "1441bb5b-4971-485a-bbbc-040b1ffc3fb0",
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
              "id": "25f0743f-a6ed-4f0e-8354-05183a200c65"
            }
          ]
        },
        {
          "id": "930f03b1-83ae-4e00-81d2-766b15c11bb8",
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
              "id": "baf47549-a5c5-494f-b27b-5bbbf0d77865"
            }
          ]
        },
        {
          "id": "1ecb954a-9083-4a9a-a3ea-717b184becd0",
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
              "id": "9e3f2668-e7f8-4f58-a218-9fc10d68e738"
            }
          ]
        },
        {
          "id": "ea8c9d9c-50d4-45f9-8e19-d144d7318b85",
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
              "id": "df88bcb4-4b55-44fb-b3aa-4f9e6683d293"
            }
          ]
        },
        {
          "id": "46577866-f119-4da5-b818-90cd8d46ae0d",
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
              "id": "681f0b8f-eafe-488d-978e-7641da478036"
            }
          ]
        },
        {
          "id": "bfd40746-c134-4bfe-be9b-a0bc4a410a41",
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
              "id": "93e58f0c-811e-4c82-8316-669f45559ea9"
            }
          ]
        },
        {
          "id": "1e03fc23-73c3-41c9-9f28-c2d353b64b91",
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
              "id": "d4f6df16-1bc2-405b-b35a-d807d047746b"
            }
          ]
        },
        {
          "id": "b3493ba9-86d4-46c4-a57a-1244a1782d9b",
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
              "id": "57b2a4a5-2390-449c-b6b9-666c350e971c"
            }
          ]
        },
        {
          "id": "26fb8e30-b04e-483a-bf87-addf75431567",
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
              "id": "53475de1-dcef-41fe-9fe2-d57e8cddee76"
            }
          ]
        },
        {
          "id": "1e989ff6-b1a7-429f-b676-edcdf9ef0556",
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
              "id": "a8946d1f-e071-471c-970f-8e19bf6fedec"
            }
          ]
        },
        {
          "id": "d3aa1ee1-eac7-47af-b79c-b09e6a5e80ca",
          "name": "deleteEventsEvent",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DELETE events event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23fa1f8c-97d7-4986-a115-9ecbbb603ac4"
            }
          ]
        }
      ]
    }
  ]
}