---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez To send an board request email to a external provider
  version: 1.0.0
  description: To send an board request email to a external provider.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/digitalsignature/signable/remind/{eventId}:
    get:
      summary: Send a reminder for an Envelope
      description: Send a reminder for an envelope.
      operationId: DigitalSignature_RemindByeventId
      x-api-path-slug: apidigitalsignaturesignableremindeventid-get
      parameters:
      - in: path
        name: eventId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Send
      - Reminderan
      - Envelope
  /api/group/{id}/sendemail:
    post:
      summary: To send an adhoc email to a group
      description: To send an adhoc email to a group.
      operationId: Group_SendEmailByidByemailDataContract
      x-api-path-slug: apigroupidsendemail-post
      parameters:
      - in: body
        name: emailDataContract
        description: Details of the email to send
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Email
      - To
      - Group
  /api/group/{id}/sendsms:
    post:
      summary: To send an adhoc sms to a group
      description: To send an adhoc sms to a group.
      operationId: Group_SendSMSByidBysmsDataContract
      x-api-path-slug: apigroupidsendsms-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: smsDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Sms
      - To
      - Group
  /api/role/{id}/boardrequest:
    post:
      summary: To send an board request email to a external provider
      description: To send an board request email to a external provider.
      operationId: Role_BoardRequestByidByupdateBoardRequestDataContract
      x-api-path-slug: apiroleidboardrequest-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateBoardRequestDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Board
      - Request
      - Email
      - To
      - External
      - Provider
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