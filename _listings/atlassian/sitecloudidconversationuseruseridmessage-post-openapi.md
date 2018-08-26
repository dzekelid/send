---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Send message to a user
  description: Send message to a user.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/user/{userId}/message:
    post:
      summary: Send message to a user
      description: Send message to a user.
      operationId: UserMessagePostHandler
      x-api-path-slug: sitecloudidconversationuseruseridmessage-post
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
      - To
      - User
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