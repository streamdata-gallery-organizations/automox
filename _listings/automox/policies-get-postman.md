{
  "info": {
    "name": "Automox Get Policies",
    "_postman_id": "fb2ef5a0-ff50-4d9a-a4d7-26fb81c8d423",
    "description": "Gets all `Policy` objects for authenticated user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "a3420d12-e727-4340-b8e3-bba536194d54",
          "name": "gets-all-event-objects-for-the-authenticated-user",
          "request": {
            "url": "http://console.automox.com/api/events",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all `Event` objects for the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "514405f0-5625-4bd8-9861-37631e9f40d5"
            }
          ]
        },
        {
          "id": "0f788f5f-6df5-4cba-b549-82f6510c87ab",
          "name": "gets-a-specific-event-object-for-the-authenticated-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "console.automox.com",
              "path": [
                "api",
                "events/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a specific `Event` object for the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea42ced1-96f3-487b-a6d7-dfb82d2772d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Orgs",
      "item": [
        {
          "id": "cf6069a1-3123-4aa4-939a-a1af2c2a04ec",
          "name": "gets-all-organizations-for-the-api-key",
          "request": {
            "url": "http://console.automox.com/api/orgs",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all organizations for the api key"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8820d08-f7ed-40b7-b6b3-105863d0b90a"
            }
          ]
        },
        {
          "id": "7b1e132b-9c75-44a4-a835-655baded8590",
          "name": "returns-all-software-packages-discovered-on-all-servers-endpoints-of-an-organization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "console.automox.com",
              "path": [
                "api",
                "orgs/:id/packages"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all software packages discovered on all servers (endpoints) of an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66172c47-0772-4466-9535-1e4297597224"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "4615dc18-9d9a-48d3-9438-e5122741315a",
          "name": "gets-all-policy-objects-for-authenticated-user",
          "request": {
            "url": "http://console.automox.com/api/policies?o=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all `Policy` objects for authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9fc13ea-6793-41c6-aa8a-79b91ac4ce5b"
            }
          ]
        }
      ]
    }
  ]
}