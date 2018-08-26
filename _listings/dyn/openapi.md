---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 1
info:
  title: Dyn
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  send:
    post:
      summary: Send Email
      description: Sending Email
      operationId: postSend
      x-api-path-slug: send-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bcc
        description: Address(es) to blind copy the email to
      - in: query
        name: bodyhtml
        description: The text/html version of the email; this field may be encoded
          in 7-bit, 8-bit, quoted-printable, or base64
      - in: query
        name: bodytext
        description: The plain/text version of the email; this field may be encoded
          in Base64 (recommended), quoted-printable, 8-bit, or 7-bit
      - in: query
        name: cc
        description: Address(es) to copy the email to
      - in: query
        name: comments
        description: Additional comments about the message
      - in: query
        name: from
        description: Required
      - in: query
        name: importance
        description: A hint from the originator on how important the message is
      - in: query
        name: inreplyto
        description: One or more message identifier(s) of the original message(s)
          to which the current message is a reply
      - in: query
        name: keywords
        description: A comma-separated list of important words and phrases useful
          for recipient
      - in: query
        name: messageid
        description: A unique message identifier that can be passed in via the api
          and override the Dyn automatically generated message id
      - in: query
        name: priority
        description: Values are either normal, urgent, or non-urgent
      - in: query
        name: references
        description: The message identifier(s) of other message(s) to which the current
          message may be related
      - in: query
        name: replyby
        description: The date and time by which a reply is requested
      - in: query
        name: replyto
        description: The email address for the recipient to reply to
      - in: query
        name: resent-date
        description: The date and time that a message is resent in the same format
          as replyby
      - in: query
        name: resent-from
        description: The email address of the person who has resent the message, or
          on whose behalf the message has been resent
      - in: query
        name: resent-messageid
        description: Contains a message identifier for a resent message
      - in: query
        name: resent-replyto
        description: Resent Reply-to in the same format as the replyto header
      - in: query
        name: resent-sender
        description: The email address of the person who has resent the message, if
          this is different from the resent-from value
      - in: query
        name: sender
        description: This is the email address of the agent responsible for sending
          the message
      - in: query
        name: sensitivity
        description: How sensitive it is to disclose this message with values that
          can be either personal, private or company confidential
      - in: query
        name: subject
        description: Required
      - in: query
        name: to
        description: Required
      - in: query
        name: xheaders
        description: Any additional custom X-headers to send in the email
      responses:
        200:
          description: OK
      tags:
      - Send
      - Email
---