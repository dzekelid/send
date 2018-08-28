{
  "info": {
    "name": "Microsoft Graph API List Rejected Senders",
    "_postman_id": "3e101e11-c7b7-4981-a6e5-13928eac97a3",
    "description": "List rejectedSenders Get a list of users or groups that are in the rejectedSenders list for this group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "d0e45c41-d4bd-416f-880a-7fed2abd509c",
          "name": "ListRejectedSenders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/rejectedSenders"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List rejectedSenders Get a list of users or groups that are in the rejectedSenders list for this group"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "a2a28262-f30b-4f20-8121-5507bf49942a"
            }
          ]
        }
      ]
    }
  ]
}