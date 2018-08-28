---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Send
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid - Add Mail Send
  x-api-slug: mailsend-post
  description: "This endpoint allows you to send email over SendGrid???s v3 Web API,
    the most recent version of our API. If you are looking for documentation about
    the v2 Mail Send endpoint, please see our [v2 API Reference](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).\n\n*
    Top level parameters are referred to as \"global\".\n* Individual fields within
    the personalizations array will override any other global, or ???message level???,
    parameters that are defined outside of personalizations.\n \n**SendGrid provides
    libraries to help you quickly and easily integrate with the v3 Web API in 7 different
    languages: [C#](https://github.com/sendgrid/sendgrid-csharp), [Go](https://github.com/sendgrid/sendgrid-go),
    [Java](https://github.com/sendgrid/sendgrid-java), [Node JS](https://github.com/sendgrid/sendgrid-nodejs),
    [PHP](https://github.com/sendgrid/sendgrid-php), [Python](https://github.com/sendgrid/sendgrid-python),
    and [Ruby](https://github.com/sendgrid/sendgrid-ruby).**\n\n\nFor more detailed
    information about how to use the v3 Mail Send endpoint, please visit our [Classroom](https://sendgrid.com/docs/Classroom/Send/v3_Mail_Send/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/mailsend-post-openapi.md
- name: SendGrid - Delete Senders Sender
  x-api-slug: senderssender-id-delete
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid - Get Senders Sender
  x-api-slug: senderssender-id-get
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid - Patch Senders Sender
  x-api-slug: senderssender-id-patch
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid - Add Senders Sender  Resend Verification
  x-api-slug: senderssender-idresend-verification-post
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid - Get Senders
  x-api-slug: senders-get
  description: |-
    **This endpoint allows you to retrieve a list of all sender identities that have been created for your account.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-get-openapi.md
- name: SendGrid - Add Senders
  x-api-slug: senders-post
  description: |-
    **This endpoint allows you to create a new sender identity.**

    *You may create up to 100 unique sender identities.*

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-post-openapi.md
- name: SendGrid - Delete Senders Sender
  x-api-slug: senderssender-id-delete
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid - Get Senders Sender
  x-api-slug: senderssender-id-get
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid - Patch Senders Sender
  x-api-slug: senderssender-id-patch
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid - Add Senders Sender  Resend Verification
  x-api-slug: senderssender-idresend-verification-post
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid - Get User Scheduled Sends
  x-api-slug: userscheduled-sends-get
  description: |-
    **This endpoint allows you to retrieve all cancel/paused scheduled send information.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sends-get-openapi.md
- name: SendGrid - Add User Scheduled Sends
  x-api-slug: userscheduled-sends-post
  description: |-
    **This endpoint allows you to cancel or pause an email that has been scheduled to be sent.**

    If the maximum number of cancellations/pauses are added, HTTP 400 will
    be returned.

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sends-post-openapi.md
- name: SendGrid - Delete User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-delete
  description: |-
    **This endpoint allows you to delete the cancellation/pause of a scheduled send.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-delete-openapi.md
- name: SendGrid - Get User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-get
  description: |-
    **This endpoint allows you to retrieve the cancel/paused scheduled send information for a specific `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-get-openapi.md
- name: SendGrid - Patch User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-patch
  description: |-
    **This endpoint allows you to update the status of a scheduled send for the given `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-patch-openapi.md
- name: SendGrid - Get Api Keys
  x-api-slug: api-keys-get
  description: |-
    **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keys-get-openapi.md
- name: SendGrid - Add Api Keys
  x-api-slug: api-keys-post
  description: |-
    **This endpoint allows you to create a new random API Key for the user.**

    A JSON request body containing a "name" property is required. If number of maximum keys is reached, HTTP 403 will be returned.

    There is a limit of 100 API Keys on your account.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    See the [API Key Permissions List](https://sendgrid.com/docs/API_Reference/Web_API_v3/API_Keys/api_key_permissions_list.html) for a list of all available scopes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keys-post-openapi.md
- name: SendGrid - Delete Api Keys Api Key
  x-api-slug: api-keysapi-key-id-delete
  description: |-
    **This endpoint allows you to revoke an existing API Key**

    Authentications using this API Key will fail after this request is made, with some small propogation delay.If the API Key ID does not exist an HTTP 404 will be returned.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    ## URI Parameters

    | URI Parameter   | Type  | Required?  | Description  |
    |---|---|---|---|
    |api_key_id |string | required | The ID of the API Key you are deleting.|
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keysapi-key-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keysapi-key-id-delete-openapi.md
- name: SendGrid - Patch Api Keys Api Key
  x-api-slug: api-keysapi-key-id-patch
  description: |-
    **This endpoint allows you to update the name of an existing API Key.**

    A JSON request body with a "name" property is required.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    ## URI Parameters

    | URI Parameter   | Type  | Required?  | Description  |
    |---|---|---|---|
    |api_key_id |string | required | The ID of the API Key you are updating.|
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keysapi-key-id-patch-openapi.md
- name: SendGrid - Put Api Keys Api Key
  x-api-slug: api-keysapi-key-id-put
  description: |-
    **This endpoint allows you to update the name and scopes of a given API key.**

    A JSON request body with a "name" property is required.
    Most provide the list of all the scopes an api key should have.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/api-keysapi-key-id-put-openapi.md
- name: SendGrid - Delete Senders Sender
  x-api-slug: senderssender-id-delete
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid - Get Senders Sender
  x-api-slug: senderssender-id-get
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid - Patch Senders Sender
  x-api-slug: senderssender-id-patch
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid - Add Senders Sender  Resend Verification
  x-api-slug: senderssender-idresend-verification-post
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid - Get Senders
  x-api-slug: senders-get
  description: |-
    **This endpoint allows you to retrieve a list of all sender identities that have been created for your account.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-get-openapi.md
- name: SendGrid - Add Senders
  x-api-slug: senders-post
  description: |-
    **This endpoint allows you to create a new sender identity.**

    *You may create up to 100 unique sender identities.*

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-post-openapi.md
- name: SendGrid - Delete Senders Sender
  x-api-slug: senderssender-id-delete
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid - Get Senders Sender
  x-api-slug: senderssender-id-get
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid - Patch Senders Sender
  x-api-slug: senderssender-id-patch
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid - Add Senders Sender  Resend Verification
  x-api-slug: senderssender-idresend-verification-post
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid - Get User Scheduled Sends
  x-api-slug: userscheduled-sends-get
  description: |-
    **This endpoint allows you to retrieve all cancel/paused scheduled send information.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sends-get-openapi.md
- name: SendGrid - Add User Scheduled Sends
  x-api-slug: userscheduled-sends-post
  description: |-
    **This endpoint allows you to cancel or pause an email that has been scheduled to be sent.**

    If the maximum number of cancellations/pauses are added, HTTP 400 will
    be returned.

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sends-post-openapi.md
- name: SendGrid - Delete User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-delete
  description: |-
    **This endpoint allows you to delete the cancellation/pause of a scheduled send.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-delete-openapi.md
- name: SendGrid - Get User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-get
  description: |-
    **This endpoint allows you to retrieve the cancel/paused scheduled send information for a specific `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-get-openapi.md
- name: SendGrid - Patch User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-patch
  description: |-
    **This endpoint allows you to update the status of a scheduled send for the given `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-patch-openapi.md
- name: SendGrid - Add Senders Sender  Resend Verification
  x-api-slug: senderssender-idresend-verification-post
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid - Patch Senders Sender
  x-api-slug: senderssender-id-patch
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid - Get Senders Sender
  x-api-slug: senderssender-id-get
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid - Delete Senders Sender
  x-api-slug: senderssender-id-delete
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid - Add Senders Sender  Resend Verification
  x-api-slug: senderssender-idresend-verification-post
  description: |-
    **This enpdoint allows you to resend a sender identity verification email.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-idresend-verification-post-openapi.md
- name: SendGrid - Patch Senders Sender
  x-api-slug: senderssender-id-patch
  description: |-
    **This endpoint allows you to update a sender identity.**

    Updates to `from.email` require re-verification. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.

    Partial updates are allowed, but fields that are marked as "required" in the POST (create) endpoint must not be nil if that field is included in the PATCH request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-patch-openapi.md
- name: SendGrid - Get Senders Sender
  x-api-slug: senderssender-id-get
  description: |-
    **This endpoint allows you to retrieve a specific sender identity.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-get-openapi.md
- name: SendGrid - Delete Senders Sender
  x-api-slug: senderssender-id-delete
  description: |-
    **This endoint allows you to delete one of your sender identities.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senderssender-id-delete-openapi.md
- name: SendGrid - Add Senders
  x-api-slug: senders-post
  description: |-
    **This endpoint allows you to create a new sender identity.**

    *You may create up to 100 unique sender identities.*

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-post-openapi.md
- name: SendGrid - Get Senders
  x-api-slug: senders-get
  description: |-
    **This endpoint allows you to retrieve a list of all sender identities that have been created for your account.**

    Sender Identities are required to be verified before use. If your domain has been whitelabeled it will auto verify on creation. Otherwise an email will be sent to the `from.email`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/senders-get-openapi.md
- name: SendGrid - Patch User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-patch
  description: |-
    **This endpoint allows you to update the status of a scheduled send for the given `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-patch-openapi.md
- name: SendGrid - Get User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-get
  description: |-
    **This endpoint allows you to retrieve the cancel/paused scheduled send information for a specific `batch_id`.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-get-openapi.md
- name: SendGrid - Delete User Scheduled Sends Batch
  x-api-slug: userscheduled-sendsbatch-id-delete
  description: |-
    **This endpoint allows you to delete the cancellation/pause of a scheduled send.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sendsbatch-id-delete-openapi.md
- name: SendGrid - Add User Scheduled Sends
  x-api-slug: userscheduled-sends-post
  description: |-
    **This endpoint allows you to cancel or pause an email that has been scheduled to be sent.**

    If the maximum number of cancellations/pauses are added, HTTP 400 will
    be returned.

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sends-post-openapi.md
- name: SendGrid - Get User Scheduled Sends
  x-api-slug: userscheduled-sends-get
  description: |-
    **This endpoint allows you to retrieve all cancel/paused scheduled send information.**

    The Cancel Scheduled Sends feature allows the customer to cancel a scheduled send based on a Batch ID included in the SMTPAPI header. Scheduled sends cancelled less than 10 minutes before the scheduled time are not guaranteed to be cancelled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/sendgrid/userscheduled-sends-get-openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-api-gallery
  url: http://school.digger.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sendgrid.stack.network
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---