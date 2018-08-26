---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Send Mail
  description: Send mail Send the message specified in the request body. The message
    is saved in the Sent Items folder by default.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/messages/{id}/send:
    post:
      summary: Message Send
      description: 'message: send Send a message in the draft folder. The draft message
        can be a new message draft, reply draft, reply-all draft, or a forward draft.
        The message is then saved in the Sent Items folder.'
      operationId: Message:Send
      x-api-path-slug: memessagesidsend-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Send
  /users/{id | userPrincipalName}/messages/{id}/send:
    post:
      summary: Message Send
      description: 'message: send Send a message in the draft folder. The draft message
        can be a new message draft, reply draft, reply-all draft, or a forward draft.
        The message is then saved in the Sent Items folder.'
      operationId: Message:Send
      x-api-path-slug: usersid--userprincipalnamemessagesidsend-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Send
  /users/{id | userPrincipalName}/sendMail:
    post:
      summary: Send Mail
      description: Send mail Send the message specified in the request body. The message
        is saved in the Sent Items folder by default.
      operationId: SendMail
      x-api-path-slug: usersid--userprincipalnamesendmail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send
      - Mail
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---