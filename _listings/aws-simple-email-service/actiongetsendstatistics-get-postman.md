{
  "info": {
    "name": "AWS Simple Email Service API Get Send Statistics",
    "_postman_id": "c91f433a-9c25-41c8-bc32-87b983314519",
    "description": "Returns the user's sending statistics.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "e12d9acf-60ed-469d-8aaf-727f69cc9e3a",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20664302-50f4-4425-9548-0f161c515780"
            }
          ]
        }
      ]
    }
  ]
}