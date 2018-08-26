---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Rejected Senders
  description: List rejectedSenders Get a list of users or groups that are in the
    rejectedSenders list for this group.
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
  /groups/{id}/acceptedSenders/$ref:
    delete:
      summary: Remove Accepted Sender
      description: Remove acceptedSender Remove a user or group from the acceptedSenders
        list.
      operationId: RemoveAcceptedSender
      x-api-path-slug: groupsidacceptedsendersref-delete
      parameters:
      - in: query
        name: $id
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: gt;
        type: string
      - in: path
        name: id
        type: string
      - in: query
        name: lt;id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Accepted
      - Sender
    post:
      summary: Create Accepted Sender
      description: Create acceptedSender Add a new user or group to the acceptedSender
        list.
      operationId: CreateAcceptedSender
      x-api-path-slug: groupsidacceptedsendersref-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accepted
      - Sender
  /groups/{id}/rejectedSenders/$ref:
    delete:
      summary: Remove Rejected Sender
      description: Remove rejectedSender Remove a user or group from the rejectedSenders
        list.
      operationId: RemoveRejectedSender
      x-api-path-slug: groupsidrejectedsendersref-delete
      parameters:
      - in: query
        name: $id
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: gt;
        type: string
      - in: path
        name: id
        type: string
      - in: query
        name: lt;id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Rejected
      - Sender
    post:
      summary: Create Rejected Sender
      description: Create rejectedSender Add a new user or group to the rejectedSender
        list.
      operationId: CreateRejectedSender
      x-api-path-slug: groupsidrejectedsendersref-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rejected
      - Sender
  /groups/{id}/acceptedSenders:
    get:
      summary: List Accepted Senders
      description: List acceptedSenders Get a list of users or groups that are in
        the acceptedSenders list for this group.
      operationId: ListAcceptedSenders
      x-api-path-slug: groupsidacceptedsenders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Accepted
      - Senders
  /groups/{id}/rejectedSenders:
    get:
      summary: List Rejected Senders
      description: List rejectedSenders Get a list of users or groups that are in
        the rejectedSenders list for this group.
      operationId: ListRejectedSenders
      x-api-path-slug: groupsidrejectedsenders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Rejected
      - Senders
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