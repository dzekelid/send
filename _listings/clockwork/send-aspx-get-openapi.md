---
swagger: "2.0"
x-collection-name: Clockwork
x-complete: 0
info:
  title: Clockwork SMS Send SMS Via HTTP
  description: The HTTP interface to send text messages can be accessed using GET
    or POST. All parameters must be URL Encoded and sent as UTF-8 text.
  termsOfService: http://www.clockworksms.com/terms-and-conditions/
  version: v1
host: api.clockworksms.com
basePath: http/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  send.aspx:
    get:
      summary: Send SMS Via HTTP
      description: The HTTP interface to send text messages can be accessed using
        GET or POST. All parameters must be URL Encoded and sent as UTF-8 text.
      operationId: getSend.aspx
      x-api-path-slug: send-aspx-get
      parameters:
      - in: query
        name: Content
        description: The message you want to send
      - in: query
        name: From
        description: The text or phone number displayed when a text message is received
          on a phone
      - in: query
        name: Key
        description: Your API key, available by logging in (with your username and
          password) to Clockwork
      - in: query
        name: Long
        description: Set this to 1 and weu2019ll stick together multiple messages
          giving you up to 459 characters, rather than the standard 160 (each recipient
          will cost up to 3 message credits)
      - in: query
        name: total
        description: Up to 50 comma separated numbers
      responses:
        200:
          description: OK
      tags:
      - Send
      - SMS
      - Via
      - HTTP
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