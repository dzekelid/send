{
  "info": {
    "name": "Microsoft Office 365 Add Messages Event Send",
    "_postman_id": "d85b4638-57d7-45c7-83e2-04aaa78219ce",
    "description": "You can send an existing email that has the IsDraft property...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "messages",
      "item": [
        {
          "id": "cb14002c-10fa-40d6-8e15-c982bd37246a",
          "name": "postMessagesEventSend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "Messages:event_id/Send"
              ],
              "variable": [
                {
                  "id": "event_id",
                  "value": "event_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "You can send an existing email that has the IsDraft property"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d278ed97-003b-451c-8c74-67fa085b88b4"
            }
          ]
        }
      ]
    }
  ]
}