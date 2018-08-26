---
swagger: "2.0"
x-collection-name: Mailgun
x-complete: 1
info:
  title: Mailgun API
  description: powerful-apis-that-allow-you-to-send-receive-and-track-email-effortlessly-
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  messages/:
    post:
      summary: Send Message
      description: Sends a message by assembling it from the components. Note that
        you can specify most parameters multiple times, HTTP supports this out of
        the box. This makes sense for parameters like cc, to or attachment.
      operationId: postMessages
      x-api-path-slug: messages-post
      parameters:
      - in: query
        name: attachment
        description: File attachment
      - in: query
        name: bcc
        description: Same as To but for Bcc
      - in: query
        name: cc
        description: Same as To but for Cc
      - in: query
        name: from
        description: Email address for From header
      - in: query
        name: h:X-My-Header
        description: 'h: prefix followed by an arbitrary value allows to appendna
          custom MIME header to the message (X-My-Headernin this case)'
      - in: query
        name: html
        description: Body of the message
      - in: query
        name: inline
        description: Attachment with inline disposition
      - in: query
        name: o:campaign
        description: Id of the campaign the message belongs to
      - in: query
        name: o:deliverytime
        description: Desired time of delivery
      - in: query
        name: o:dkim
        description: Enables/disables DKIM signatures on per-message basis
      - in: query
        name: o:tag
        description: Tag string
      - in: query
        name: o:testmode
        description: Enables sending in test mode
      - in: query
        name: o:tracking
        description: Toggles tracking on a per-message basis, seenTracking Messages
          for details
      - in: query
        name: o:tracking-clicks
        description: Toggles clicks tracking on a per-message basis
      - in: query
        name: o:tracking-opens
        description: Toggles opens tracking on a per-message basis
      - in: query
        name: subject
        description: Message subject
      - in: query
        name: text
        description: Body of the message
      - in: query
        name: to
        description: Email address of the recipient(s)
      - in: query
        name: v:my-var
        description: 'v: prefix followed by an arbitrary name allows tonattach a custom
          JSON data to the message'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
---