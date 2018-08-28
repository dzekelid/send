---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Gigme Phone Send
  version: 1.0.0
  description: Post gigme phone send.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/email/send:
    post:
      summary: Post Email Send
      description: Post email send.
      operationId: postApiV1EmailSend
      x-api-path-slug: apiv1emailsend-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Send
  /api/v1/gigme/email/send:
    post:
      summary: Post Gigme Email Send
      description: Post gigme email send.
      operationId: postApiV1GigmeEmailSend
      x-api-path-slug: apiv1gigmeemailsend-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Email
      - Send
  /api/v1/gigme/phone/send:
    post:
      summary: Post Gigme Phone Send
      description: Post gigme phone send.
      operationId: postApiV1GigmePhoneSend
      x-api-path-slug: apiv1gigmephonesend-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Phone
      - Send
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