---
name: Postmark
x-slug: postmark
description: Trusted by thousands of developers, Postmark is a fast and reliable transactional
  email service. Send with Postmark to ensure your transactional emails get to the
  inbox on time, every time.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
x-kinRank: "8"
x-alexaRank: "87545"
tags: Send
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/apis.md
specificationVersion: "0.14"
apis:
- name: Postmark - Get Stats Outbound Sends
  x-api-slug: statsoutboundsends-get
  description: Get stats outbound sends.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/statsoutboundsends-get-openapi.md
- name: Postmark - Get Stats Outbound Sends
  x-api-slug: statsoutboundsends-get
  description: Get stats outbound sends.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/statsoutboundsends-get-openapi.md
- name: Postmark - Get Stats Outbound Sends
  x-api-slug: statsoutboundsends-get
  description: Get stats outbound sends.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/statsoutboundsends-get-openapi.md
- name: Postmark Account-level - List Sender Signatures
  x-api-slug: senders-get
  description: List sender signatures.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senders-get-openapi.md
- name: Postmark Account-level - Create a Sender Signature
  x-api-slug: senders-post
  description: Create a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senders-post-openapi.md
- name: Postmark Account-level - Delete a Sender Signature
  x-api-slug: senderssignatureid-delete
  description: Delete a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-delete-openapi.md
- name: Postmark Account-level - Get a Sender Signature
  x-api-slug: senderssignatureid-get
  description: Get a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-get-openapi.md
- name: Postmark Account-level - Update a Sender Signature
  x-api-slug: senderssignatureid-put
  description: Update a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-put-openapi.md
- name: Postmark Account-level - Request a new DKIM Key
  x-api-slug: senderssignatureidrequestnewdkim-post
  description: "Requests a new DKIM key to be created. Until the DNS entries are confirmed,
    \nthe new values will be in the `DKIMPendingHost` and `DKIMPendingTextValue` fields.
    \nAfter the new DKIM value is verified in DNS, the pending values will migrate
    to \n`DKIMTextValue` and `DKIMPendingTextValue` and Postmark will begin to sign
    emails \nwith the new DKIM key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidrequestnewdkim-post-openapi.md
- name: Postmark Account-level - Resend Signature Confirmation Email
  x-api-slug: senderssignatureidresend-post
  description: Resend signature confirmation email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidresend-post-openapi.md
- name: Postmark Account-level - Request DNS Verification for SPF
  x-api-slug: senderssignatureidverifyspf-post
  description: Request dns verification for spf.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidverifyspf-post-openapi.md
- name: Postmark Account-level - List Sender Signatures
  x-api-slug: senders-get
  description: List sender signatures.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senders-get-openapi.md
- name: Postmark Account-level - Create a Sender Signature
  x-api-slug: senders-post
  description: Create a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senders-post-openapi.md
- name: Postmark Account-level - Delete a Sender Signature
  x-api-slug: senderssignatureid-delete
  description: Delete a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-delete-openapi.md
- name: Postmark Account-level - Get a Sender Signature
  x-api-slug: senderssignatureid-get
  description: Get a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-get-openapi.md
- name: Postmark Account-level - Update a Sender Signature
  x-api-slug: senderssignatureid-put
  description: Update a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-put-openapi.md
- name: Postmark Account-level - Request a new DKIM Key
  x-api-slug: senderssignatureidrequestnewdkim-post
  description: "Requests a new DKIM key to be created. Until the DNS entries are confirmed,
    \nthe new values will be in the `DKIMPendingHost` and `DKIMPendingTextValue` fields.
    \nAfter the new DKIM value is verified in DNS, the pending values will migrate
    to \n`DKIMTextValue` and `DKIMPendingTextValue` and Postmark will begin to sign
    emails \nwith the new DKIM key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidrequestnewdkim-post-openapi.md
- name: Postmark Account-level - Resend Signature Confirmation Email
  x-api-slug: senderssignatureidresend-post
  description: Resend signature confirmation email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidresend-post-openapi.md
- name: Postmark Account-level - Request DNS Verification for SPF
  x-api-slug: senderssignatureidverifyspf-post
  description: Request dns verification for spf.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidverifyspf-post-openapi.md
- name: Postmark Account-level - Request DNS Verification for SPF
  x-api-slug: senderssignatureidverifyspf-post
  description: Request dns verification for spf.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidverifyspf-post-openapi.md
- name: Postmark Account-level - Resend Signature Confirmation Email
  x-api-slug: senderssignatureidresend-post
  description: Resend signature confirmation email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidresend-post-openapi.md
- name: Postmark Account-level - Request a new DKIM Key
  x-api-slug: senderssignatureidrequestnewdkim-post
  description: "Requests a new DKIM key to be created. Until the DNS entries are confirmed,
    \nthe new values will be in the `DKIMPendingHost` and `DKIMPendingTextValue` fields.
    \nAfter the new DKIM value is verified in DNS, the pending values will migrate
    to \n`DKIMTextValue` and `DKIMPendingTextValue` and Postmark will begin to sign
    emails \nwith the new DKIM key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureidrequestnewdkim-post-openapi.md
- name: Postmark Account-level - Update a Sender Signature
  x-api-slug: senderssignatureid-put
  description: Update a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-put-openapi.md
- name: Postmark Account-level - Get a Sender Signature
  x-api-slug: senderssignatureid-get
  description: Get a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-get-openapi.md
- name: Postmark Account-level - Delete a Sender Signature
  x-api-slug: senderssignatureid-delete
  description: Delete a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senderssignatureid-delete-openapi.md
- name: Postmark Account-level - Create a Sender Signature
  x-api-slug: senders-post
  description: Create a sender signature.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senders-post-openapi.md
- name: Postmark Account-level - List Sender Signatures
  x-api-slug: senders-get
  description: List sender signatures.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/postmark/senders-get-openapi.md
x-common:
- type: x--net-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#dot-net
- type: x-api-gallery
  url: http://polygon.api.gallery.streamdata.io
- type: x-api-stack
  url: http://postmark.stack.network
- type: x-base
  url: https://api.postmarkapp.com
- type: x-blog
  url: http://blog.postmarkapp.com/
- type: x-blog-rss
  url: http://blog.postmarkapp.com/rss
- type: x-contact-form
  url: http://support.postmarkapp.com/customer/portal/emails/new
- type: x-crunchbase
  url: https://crunchbase.com/organization/postmark
- type: x-crunchbase
  url: http://www.crunchbase.com/company/postmark
- type: x-developer
  url: http://developer.postmarkapp.com/
- type: x-email
  url: support@postmarkapp.com
- type: x-email
  url: 451d9b70cf9364d23ff6f9d51d870251569e+ahoy@inbound.postmarkapp.com
- type: x-faq
  url: http://support.postmarkapp.com/
- type: x-pricing
  url: http://developer.postmarkapp.com/developer-api-messages.html
- type: x-privacy
  url: https://postmarkapp.com/privacy-policy
- type: x-ruby-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#rails
- type: x-ruby-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#ruby
- type: x-selfservice-registration
  url: https://postmarkapp.com/sign_up
- type: x-status
  url: http://status.postmarkapp.com/
- type: x-terms-of-service
  url: https://postmarkapp.com/terms-of-service
- type: x-twitter
  url: https://twitter.com/postmarkapp
- type: x-website
  url: http://postmarkapp.com
- type: x-website
  url: http://postmarkapp.com/
- type: x-website
  url: https://postmarkapp.com
- type: x-wordpress-pdk
  url: http://developer.postmarkapp.com/developer-official-libs.html#wordpress
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---