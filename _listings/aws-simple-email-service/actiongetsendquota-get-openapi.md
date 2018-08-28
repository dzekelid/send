---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Get Send Quota
  version: 1.0.0
  description: Returns the user's current sending limits.
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
  /?Action=SendEmail:
    get:
      summary: Send Email
      description: Composes an email message based on input data, and then immediately
        queues the message for sending.
      operationId: sendEmail
      x-api-path-slug: actionsendemail-get
      parameters:
      - in: query
        name: ConfigurationSetName
        description: The name of the configuration set to use when you send an email
          using SendEmail
        type: string
      - in: query
        name: Destination
        description: 'The destination for this email, composed of To:, CC:, and BCC:
          fields'
        type: string
      - in: query
        name: Message
        description: The message to be sent
        type: string
      - in: query
        name: ReplyToAddresses.member.N
        description: The reply-to email address(es) for the message
        type: string
      - in: query
        name: ReturnPath
        description: The email address to which bounces and complaints are to be forwarded
          when feedback forwarding is enabled
        type: string
      - in: query
        name: ReturnPathArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Source
        description: The email address that is sending the email
        type: string
      - in: query
        name: SourceArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Tags.member.N
        description: A list of tags, in the form of name/value pairs, to apply to
          an email that you send using SendEmail
        type: string
      responses:
        200:
          description: OK
      tags:
      - Email
  /?Action=SendRawEmail:
    get:
      summary: Send Raw Email
      description: Sends an email message, with header and content specified by the
        client.
      operationId: sendRawEmail
      x-api-path-slug: actionsendrawemail-get
      parameters:
      - in: query
        name: ConfigurationSetName
        description: The name of the configuration set to use when you send an email
          using SendRawEmail
        type: string
      - in: query
        name: Destinations.member.N
        description: 'A list of destinations for the message, consisting of To:, CC:,
          and BCC: addresses'
        type: string
      - in: query
        name: FromArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: RawMessage
        description: The raw text of the message
        type: string
      - in: query
        name: ReturnPathArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Source
        description: The identitys email address
        type: string
      - in: query
        name: SourceArn
        description: This parameter is used only for sending authorization
        type: string
      - in: query
        name: Tags.member.N
        description: A list of tags, in the form of name/value pairs, to apply to
          an email that you send using SendRawEmail
        type: string
      responses:
        200:
          description: OK
      tags:
      - Email
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