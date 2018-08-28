swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
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
  /trackerCommands:
    post:
      summary: Tracker command sending
      description: Sends a downlink command to a supported Abeeway tracker.
      operationId: sends-a-downlink-command-to-a-supported-abeeway-tracker
      x-api-path-slug: trackercommands-post
      parameters:
      - in: body
        name: trackerCommand
        description: Contents of the tracker command
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tracker
      - Command
      - Sending