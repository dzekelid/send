swagger: "2.0"
x-collection-name: Flowroute
x-complete: 1
info:
  title: Flowroute APIs
  description: the-flowroute-apis-are-organized-around-rest--our-apis-have-resourceoriented-urls-support-http-verbs-and-respond-with-http-status-codes--all-api-requests-and-responses-including-errors-will-be-represented-as-json-objects--you-can-use-the-flowroute-apis-to-manage-your-flowroute-phone-numbers-including-setting-primary-and-failover-routes-for-inbound-calls-and-sending-text-messages-sms-and-mms-using-longcode-or-tollfree-numbers-in-your-account-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2.1/messages:
    post:
      summary: Send a Message
      description: Sends an SMS or MMS from a Flowroute long code or toll-free phone
        number to another valid phone number.
      operationId: sends-an-sms-or-mms-from-a-flowroute-long-code-or-tollfree-phone-number-to-another-valid-phone-numbe
      x-api-path-slug: v2-1messages-post
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Send
      - Message