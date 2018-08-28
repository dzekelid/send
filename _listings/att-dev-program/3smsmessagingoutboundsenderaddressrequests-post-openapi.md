---
swagger: "2.0"
x-collection-name: AT&T Dev Program
x-complete: 0
info:
  title: AT&T API Post SMS Outbound Senderaddress Requests
  description: /3/smsmessaging/outbound/{senderAddress}/requests
  version: "1"
host: api.att.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3/messaging/outbound/{senderAddress}/requests:
    post:
      summary: Post Messaging Outbound Senderaddress Requests
      description: /3/messaging/outbound/{senderAddress}/requests
      operationId: 3messagingoutboundsenderaddressrequests
      x-api-path-slug: 3messagingoutboundsenderaddressrequests-post
      parameters:
      - in: path
        name: senderAddress
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Outbound
      - Senderress
      - Requests
  /3/messaging/outbound/{senderAddress}/{requestId}/deliveryInfos:
    get:
      summary: Get Messaging Outbound Senderaddress Requestid Deliveryinfos
      description: /3/messaging/outbound/{senderAddress}/{requestId}/deliveryInfos
      operationId: 3messagingoutboundsenderaddressrequestiddeliveryinfos
      x-api-path-slug: 3messagingoutboundsenderaddressrequestiddeliveryinfos-get
      parameters:
      - in: path
        name: requestId
      - in: path
        name: senderAddress
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Outbound
      - Senderress
      - RequestId
      - DeliveryInfos
  /3/smsmessaging/outbound/requests/{senderAddress}/{requestId}/deliveryInfos:
    get:
      summary: Get SMS Outbound Requests Senderaddress Requestid Deliveryinfos
      description: /3/smsmessaging/outbound/requests/{senderAddress}/{requestId}/deliveryInfos
      operationId: 3smsmessagingoutboundrequestssenderaddressrequestiddeliveryinfos
      x-api-path-slug: 3smsmessagingoutboundrequestssenderaddressrequestiddeliveryinfos-get
      parameters:
      - in: path
        name: requestId
      - in: path
        name: senderAddress
      responses:
        200:
          description: OK
      tags:
      - Smsmessaging
      - Outbound
      - Requests
      - Senderress
      - RequestId
      - DeliveryInfos
  /3/smsmessaging/outbound/{senderAddress}/requests:
    post:
      summary: Post SMS Outbound Senderaddress Requests
      description: /3/smsmessaging/outbound/{senderAddress}/requests
      operationId: 3smsmessagingoutboundsenderaddressrequests
      x-api-path-slug: 3smsmessagingoutboundsenderaddressrequests-post
      parameters:
      - in: path
        name: senderAddress
      responses:
        200:
          description: OK
      tags:
      - Smsmessaging
      - Outbound
      - Senderress
      - Requests
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