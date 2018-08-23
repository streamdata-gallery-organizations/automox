{
  "info": {
    "name": "Automox Get Events",
    "_postman_id": "7c173d3d-a7f2-4e99-a924-16095b3ea7ef",
    "description": "Gets a specific `Event` object for the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "bfd606f6-ac61-47f9-8ab6-49d22a1e23dc",
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
              "id": "b2b314f6-8419-456c-bb86-783505259dd9"
            }
          ]
        },
        {
          "id": "390deda8-399c-43a5-8e29-52d7cb0870c9",
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
              "id": "8337e43b-f4a0-46be-aba8-315c66580ab0"
            }
          ]
        }
      ]
    }
  ]
}