---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Downlink message sending
  description: Sends a new downlink message to the device, if that device is within
    authorized scopes. The message is queued in the LRC until the device is able to
    retrieve it (depending on its configured class).
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/{device}/downlinkMessages:
    post:
      summary: Downlink message sending
      description: Sends a new downlink message to the device, if that device is within
        authorized scopes. The message is queued in the LRC until the device is able
        to retrieve it (depending on its configured class).
      operationId: sends-a-new-downlink-message-to-the-device-if-that-device-is-within-authorized-scopes-the-message-is
      x-api-path-slug: devicesdevicedownlinkmessages-post
      parameters:
      - in: query
        name: confirmDownlink
        description: Indicates to send a downlink reception confirmation
      - in: path
        name: device
        description: Ref or DevEUI of the device to which the downlink message should
          be sent
      - in: query
        name: flushDownlinkQueue
        description: Indicates to flush the LRC downlink queue before adding the new
          message to the queue
      - in: body
        name: message
        description: Contents of the downlink message to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Downlink
      - Message
      - Sending
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