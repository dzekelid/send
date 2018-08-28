{
  "info": {
    "name": "Twilio SendSMS",
    "_postman_id": "831e92a6-7897-4503-a7d7-5d2bf5629751",
    "description": "SendSMS",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sms messages",
      "item": [
        {
          "id": "05d1f2fd-c48e-4a02-b4c3-b425dae9d047",
          "name": "sendsms",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/SMS/Messages.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "SendSMS"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"messages\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 201,
              "name": "Response_201",
              "id": "a3b523bd-9874-4ca1-aa63-ab8ae8635d27"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The data given in the POST or PUT failed validation",
              "code": 400,
              "name": "Response_400",
              "id": "de26df68-81c3-48a3-9f7c-fa81d581c566"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The supplied credentials, if any, are not sufficient to create or update the resource",
              "code": 401,
              "name": "Response_401",
              "id": "3545de43-5f95-4144-ade7-7d72873f93b5"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You know this one",
              "code": 404,
              "name": "Response_404",
              "id": "170c9e87-419d-447a-9e30-51bb1a4e045e"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You can't POST or PUT to the resource",
              "code": 405,
              "name": "Response_405",
              "id": "c8740d0a-f68b-40fa-8f95-94400dc3b50f"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "Your application is sending too many simultaneous requests",
              "code": 429,
              "name": "Response_429",
              "id": "61b56b9a-dd68-4a6d-b85e-e8462a7d4d81"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We couldn't create or update the resource",
              "code": 500,
              "name": "Response_500",
              "id": "10740982-99f4-43b7-a77f-84a427965222"
            }
          ]
        }
      ]
    }
  ]
}