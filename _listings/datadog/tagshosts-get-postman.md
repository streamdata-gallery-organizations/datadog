{
  "info": {
    "name": "DataDog API Get Tags Hosts",
    "_postman_id": "e752bea8-c16a-4133-b018-96dd8c407251",
    "description": "Return a mapping of tags to hosts for your whole infrastructure.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "0e46be46-a371-47a6-b8e7-e03c0adac3af",
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
              "id": "b624173f-6319-4392-8837-8c976c1ef696"
            }
          ]
        },
        {
          "id": "ba880b83-ed3f-4038-a34f-6a78351f1b57",
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
              "id": "534c5bd3-d888-4618-956c-71f576e1542d"
            }
          ]
        },
        {
          "id": "d714c227-4a66-4b79-963a-25e802bbe575",
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
              "id": "a03568d9-1364-4dbd-b874-9499172a7445"
            }
          ]
        },
        {
          "id": "76102c5c-7438-4d21-a55d-d65fcb1302cb",
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
              "id": "5858a926-f0f2-41f0-936d-bf613ad159bf"
            }
          ]
        },
        {
          "id": "13c7cadc-3de0-4fc9-a2c5-b0e4c00416ca",
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
              "id": "272c9f57-a2c1-4c74-a3f4-e8e9d2482860"
            }
          ]
        },
        {
          "id": "f266ef2d-e509-4ffa-a30f-e972453e6fb5",
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
              "id": "055576c0-0eb4-46a0-b29f-d1ec59abdf61"
            }
          ]
        },
        {
          "id": "7cc6b9dc-a8b1-431e-b3fa-6674e87a96cf",
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
              "id": "4d3e6a05-9323-4345-8587-ba3c92c5ab1f"
            }
          ]
        },
        {
          "id": "d47f9fde-aa09-4e10-ab60-a6857e09f410",
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
              "id": "3c51703d-3fb2-4d8b-a7b2-62473168e0e7"
            }
          ]
        },
        {
          "id": "8eae11cf-9b8d-47f2-949c-d290461106dc",
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
              "id": "44a875ef-984d-4fc7-a0d7-94f8a24a9f53"
            }
          ]
        },
        {
          "id": "3bc2486b-7874-412c-ba87-ec73c1fc6f5f",
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
              "id": "f4b81e7c-8f93-4fef-b451-32dda5f9679a"
            }
          ]
        },
        {
          "id": "80e5b695-3d5f-4273-9855-4b96ed462bbe",
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
              "id": "d5f386d6-4964-4d34-b3c0-437c1d1a2fac"
            }
          ]
        },
        {
          "id": "45dd541a-4ba7-4c69-ab92-f55a78dacb43",
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
              "id": "20eb953f-21bb-4dd7-af38-99fe6b3e9a4d"
            }
          ]
        },
        {
          "id": "3905497d-cf5c-4007-a797-ea736d0eef68",
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
              "id": "0ffff8d7-05a2-41de-ba9e-ab9157c93dec"
            }
          ]
        },
        {
          "id": "df265bed-3832-4a61-805a-749bbb456e98",
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
              "id": "4f5adc6b-bb4b-4f96-8803-e45d8fe771ca"
            }
          ]
        },
        {
          "id": "d5345bd1-e857-43d4-9454-d3b6991b9d53",
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
              "id": "edb59db4-e3c2-4aa6-aecd-6fdeab36ee71"
            }
          ]
        },
        {
          "id": "7ada2500-2b79-4999-8e28-dfaf3d4198eb",
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
              "id": "5206adee-bc70-4bf2-b247-e283fbb839db"
            }
          ]
        },
        {
          "id": "21f2c744-fe16-40c3-a482-fb80c41e4b96",
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
              "id": "2338e7a1-683f-452d-af34-b5cbfc167e68"
            }
          ]
        }
      ]
    }
  ]
}