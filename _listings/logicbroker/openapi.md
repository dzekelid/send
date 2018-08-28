swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Product/{partnerId}/{feedId}:
    put:
      summary: Send product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_SendFeed
      x-api-path-slug: apiv1productpartneridfeedid-put
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Send
      - Product
      - Feed