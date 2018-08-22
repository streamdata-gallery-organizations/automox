{
  "info": {
    "name": "Automox Get Events",
    "_postman_id": "cf305224-bcc4-41d1-8240-6e58161edc18",
    "description": "Gets all `Event` objects for the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "b990e5fd-d648-434e-9e14-343dc106814d",
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
              "id": "dba8824d-d651-4553-80c2-4254695fd316"
            }
          ]
        }
      ]
    }
  ]
}