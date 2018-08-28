swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '{auth_id}/Message/':
    post:
      summary: Send Message
      description: This API enables you to send messages via Plivou2019s SMS service.
      operationId: postAuthMessage
      x-api-path-slug: auth-idmessage-post
      parameters:
      - in: query
        name: dst
        description: The number to which the message needs to be sent
      - in: query
        name: log
        description: If set to false, the content of this message will not be logged
          on the Plivo infrastructure and the dst value will be masked
      - in: query
        name: method
        description: The method used to call the url
      - in: query
        name: src
        description: The phone number to be used as the caller id (with the country
          code)
      - in: query
        name: text
        description: The text to send encoded in Unicode UTF-8
      - in: path
        name: This API enables you to send messages via Plivou2019s SMS service.
        description: AUTH TOKEN Your Plivo AUTH ID and AUTH TOKEN can be found when
          you login to your dashboard
      - in: query
        name: type
        description: The type of message
      - in: query
        name: url
        description: The URL to which with the status of the message is sent
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message