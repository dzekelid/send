---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Add User Scheduled Sends
  description: |-
    **This endpoint allows you to cancel or pause an email that has been scheduled to be sent.**

    If the maximum number of cancellations/pauses are added, HTTP 400 will
    be returned.

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mail/send:
    post:
      summary: Add Mail Send
      description: "This endpoint allows you to send email over SendGrid???s v3 Web
        API, the most recent version of our API. If you are looking for documentation
        about the v2 Mail Send endpoint, please see our [v2 API Reference](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).\n\n*
        Top level parameters are referred to as \"global\".\n* Individual fields within
        the personalizations array will override any other global, or ???message level???,
        parameters that are defined outside of personalizations.\n \n**SendGrid provides
        libraries to help you quickly and easily integrate with the v3 Web API in
        7 different languages: [C#](https://github.com/sendgrid/sendgrid-csharp),
        [Go](https://github.com/sendgrid/sendgrid-go), [Java](https://github.com/sendgrid/sendgrid-java),
        [Node JS](https://github.com/sendgrid/sendgrid-nodejs), [PHP](https://github.com/sendgrid/sendgrid-php),
        [Python](https://github.com/sendgrid/sendgrid-python), and [Ruby](https://github.com/sendgrid/sendgrid-ruby).**\n\n\nFor
        more detailed information about how to use the v3 Mail Send endpoint, please
        visit our [Classroom](https://sendgrid.com/docs/Classroom/Send/v3_Mail_Send/index.html)."
      operationId: mail.send.post
      x-api-path-slug: mailsend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Send
  /senders/{sender_id}:
    delete:
      summary: Delete Senders Sender
      description: |-
        **This endoint allows you to delete one of your sender identities.**

        Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
      operationId: senders.sender_id.delete
      x-api-path-slug: senderssender-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Senders
      - Sender
    get:
      summary: Get Senders Sender
      description: |-
        **This endpoint allows you to retrieve a specific sender identity.**

        Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
      operationId: senders.sender_id.get
      x-api-path-slug: senderssender-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Senders
      - Sender
    patch:
      summary: Patch Senders Sender
      description: |-
        **This endpoint allows you to update a sender identity.**

        Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

        Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
      operationId: senders.sender_id.patch
      x-api-path-slug: senderssender-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Senders
      - Sender
  /senders/{sender_id}/resend_verification:
    post:
      summary: Add Senders Sender  Resend Verification
      description: |-
        **This enpdoint allows you to resend a sender identity verification email.**

        Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
      operationId: senders.sender_id.resend_verification.post
      x-api-path-slug: senderssender-idresend-verification-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Senders
      - Sender
      - ""
      - Resend
      - Verification
  /senders:
    get:
      summary: Get Senders
      description: |-
        **This endpoint allows you to retrieve a list of all sender identities that have been created for your account.**

        Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
      operationId: senders.get
      x-api-path-slug: senders-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Senders
    post:
      summary: Add Senders
      description: |-
        **This endpoint allows you to create a new sender identity.**

        *You may create up to 100 unique sender identities.*

        Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
      operationId: POST_senders
      x-api-path-slug: senders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Senders
  /user/scheduled_sends:
    get:
      summary: Get User Scheduled Sends
      description: |-
        **This endpoint allows you to retrieve all cancel/paused scheduled send information.**

        The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
      operationId: user.scheduled_sends.get
      x-api-path-slug: userscheduled-sends-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Scheduled
      - Sends
    post:
      summary: Add User Scheduled Sends
      description: |-
        **This endpoint allows you to cancel or pause an email that has been scheduled to be sent.**

        If the maximum number of cancellations/pauses are added, HTTP 400 will
        be returned.

        The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
      operationId: user.scheduled_sends.post
      x-api-path-slug: userscheduled-sends-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Scheduled
      - Sends
  /user/scheduled_sends/{batch_id}:
    delete:
      summary: Delete User Scheduled Sends Batch
      description: |-
        **This endpoint allows you to delete the cancellation/pause of a scheduled send.**

        The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
      operationId: user.scheduled_sends.batch_id.delete
      x-api-path-slug: userscheduled-sendsbatch-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Scheduled
      - Sends
      - Batch
    get:
      summary: Get User Scheduled Sends Batch
      description: |-
        **This endpoint allows you to retrieve the cancel/paused scheduled send information for a specific `batch_id`.**

        The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
      operationId: user.scheduled_sends.batch_id.get
      x-api-path-slug: userscheduled-sendsbatch-id-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Scheduled
      - Sends
      - Batch
    patch:
      summary: Patch User Scheduled Sends Batch
      description: |-
        **This endpoint allows you to update the status of a scheduled send for the given `batch_id`.**

        The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
      operationId: user.scheduled_sends.batch_id.patch
      x-api-path-slug: userscheduled-sendsbatch-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Scheduled
      - Sends
      - Batch
  /api_keys:
    get:
      summary: Get Api Keys
      description: |-
        **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
      operationId: GET_api_keys
      x-api-path-slug: api-keys-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
    post:
      summary: Add Api Keys
      description: |-
        **This endpoint allows you to create a new random API Key for the user.**

        A JSON request body containing a "name" property is required. If number of maximum keys is reached, HTTP 403 will be returned.

        There is a limit of 100 API Keys on your account.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        See the [API Key Permissions List](https://sendgrid.com/docs/API_Reference/Web_API_v3/API_Keys/api_key_permissions_list.html) for a list of all available scopes.
      operationId: api_keys.post
      x-api-path-slug: api-keys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
  /api_keys/{api_key_id}:
    delete:
      summary: Delete Api Keys Api Key
      description: |-
        **This endpoint allows you to revoke an existing API Key**

        Authentications using this API Key will fail after this request is made, with some small propogation delay.If the API Key ID does not exist an HTTP 404 will be returned.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        ## URI Parameters

        | URI Parameter   | Type  | Required?  | Description  |
        |---|---|---|---|
        |api_key_id |string | required | The ID of the API Key you are deleting.|
      operationId: api_keys.api_key_id.delete
      x-api-path-slug: api-keysapi-key-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
    patch:
      summary: Patch Api Keys Api Key
      description: |-
        **This endpoint allows you to update the name of an existing API Key.**

        A JSON request body with a "name" property is required.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        ## URI Parameters

        | URI Parameter   | Type  | Required?  | Description  |
        |---|---|---|---|
        |api_key_id |string | required | The ID of the API Key you are updating.|
      operationId: api_keys.api_key_id.patch
      x-api-path-slug: api-keysapi-key-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
    put:
      summary: Put Api Keys Api Key
      description: |-
        **This endpoint allows you to update the name and scopes of a given API key.**

        A JSON request body with a "name" property is required.
        Most provide the list of all the scopes an api key should have.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
      operationId: api_keys.api_key_id.put
      x-api-path-slug: api-keysapi-key-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
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