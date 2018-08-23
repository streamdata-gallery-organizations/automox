{
  "info": {
    "name": "Automox Get Orgs",
    "_postman_id": "3ce17a48-5235-4c2a-8ee1-732fc7f7fe59",
    "description": "Gets all organizations for the api key",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "c41f19b0-a884-4557-b40a-171ea20a6417",
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
              "id": "ae89f6d5-7bee-4cee-8957-abf056606610"
            }
          ]
        },
        {
          "id": "c02e6be6-7081-48af-b227-647113f873f4",
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
              "id": "b684d16e-a1a1-45c8-a176-eff32e99b61b"
            }
          ]
        }
      ]
    },
    {
      "name": "Orgs",
      "item": [
        {
          "id": "7524a7d2-f85b-4a9d-a816-a0f7fae94aae",
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
              "id": "2e6fcb95-03c5-40de-8597-bca2c9349c0b"
            }
          ]
        }
      ]
    }
  ]
}