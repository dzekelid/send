---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Send Bounce
  version: 1.0.0
  description: Generates and sends a bounce message to the sender of an email you
    received through Amazon SES.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetSendQuota:
    get:
      summary: Get Send Quota
      description: Returns the user's current sending limits.
      operationId: getSendQuota
      x-api-path-slug: actiongetsendquota-get
      parameters:
      - in: query
        name: Max24HourSend
        description: The maximum number of emails the user is allowed to send in a
          24-hour interval
        type: string
      - in: query
        name: MaxSendRate
        description: The maximum number of emails that Amazon SES can accept from
          the users account per second
        type: string
      - in: query
        name: SentLast24Hours
        description: The number of emails sent during the previous 24 hours
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send Quota
  /?Action=GetSendStatistics:
    get:
      summary: Get Send Statistics
      description: Returns the user's sending statistics.
      operationId: getSendStatistics
      x-api-path-slug: actiongetsendstatistics-get
      parameters:
      - in: query
        name: SendDataPoints.member.N
        description: A list of data points, each of which represents 15 minutes of
          activity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send Statistics
  /?Action=SendBounce:
    get:
      summary: Send Bounce
      description: Generates and sends a bounce message to the sender of an email
        you received through Amazon SES.
      operationId: sendBounce
      x-api-path-slug: actionsendbounce-get
      parameters:
      - in: query
        name: BouncedRecipientInfoList.member.N
        description: A list of recipients of the bounced message, including the information
          required to create the Delivery Status Notifications (DSNs) for the recipients
        type: string
      - in: query
        name: BounceSender
        description: The address to use in the From header of the bounce message
        type: string
      - in: query
        name: BounceSenderArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Explanation
        description: Human-readable text for the bounce message to explain the failure
        type: string
      - in: query
        name: MessageDsn
        description: Message-related DSN fields
        type: string
      - in: query
        name: OriginalMessageId
        description: The message ID of the message to be bounced
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bounce
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