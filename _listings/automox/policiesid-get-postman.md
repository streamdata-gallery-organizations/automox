{
  "info": {
    "name": "Automox Get Policies",
    "_postman_id": "e457b8a7-2e96-4aa6-b0ef-6bba90765388",
    "description": "Gets a specific `Policy` object for the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "8ac69b40-c06b-45e9-8df2-8715676b410b",
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
              "id": "bd81b21a-657b-4de7-a944-1e698ea9fe5a"
            }
          ]
        },
        {
          "id": "8222d86e-a37d-4c72-b69d-8fc5e80fd95b",
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
              "id": "4772c3dc-6de4-4cea-9809-5051478abc8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Orgs",
      "item": [
        {
          "id": "5bbd6cf0-0922-419c-9d34-f86fabdabf10",
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
              "id": "aa29f8f2-3e62-40bc-a7de-f1353f048d62"
            }
          ]
        },
        {
          "id": "f564d94e-109e-4342-8b41-f19c386e7b17",
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
              "id": "969304ec-1a37-43c9-b3d7-fcb3651df317"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "4275c417-b838-4e4c-9020-b9ca355b3bcd",
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
              "id": "e35e019a-d189-49c5-85ba-79f4250230b9"
            }
          ]
        },
        {
          "id": "016b4421-cf25-4556-be89-3d7ecae4ff34",
          "name": "gets-a-specific-policy-object-for-the-authenticated-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "console.automox.com",
              "path": [
                "api",
                "policies/:id"
              ],
              "query": [
                {
                  "key": "o",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Gets a specific `Policy` object for the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7096edb0-5600-491c-a560-e8a3365d3200"
            }
          ]
        }
      ]
    }
  ]
}