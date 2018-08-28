---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Send
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph API - Message Send
  x-api-slug: memessagesidsend-post
  description: 'message: send Send a message in the draft folder. The draft message
    can be a new message draft, reply draft, reply-all draft, or a forward draft.
    The message is then saved in the Sent Items folder.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/memessagesidsend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/memessagesidsend-post-openapi.md
- name: Microsoft Graph API - Message Send
  x-api-slug: usersid--userprincipalnamemessagesidsend-post
  description: 'message: send Send a message in the draft folder. The draft message
    can be a new message draft, reply draft, reply-all draft, or a forward draft.
    The message is then saved in the Sent Items folder.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/usersid--userprincipalnamemessagesidsend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/usersid--userprincipalnamemessagesidsend-post-openapi.md
- name: Microsoft Graph API - Send Mail
  x-api-slug: usersid--userprincipalnamesendmail-post
  description: Send mail Send the message specified in the request body. The message
    is saved in the Sent Items folder by default.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/usersid--userprincipalnamesendmail-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/usersid--userprincipalnamesendmail-post-openapi.md
- name: Microsoft Graph API - Remove Accepted Sender
  x-api-slug: groupsidacceptedsendersref-delete
  description: Remove acceptedSender Remove a user or group from the acceptedSenders
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-delete-openapi.md
- name: Microsoft Graph API - Remove Rejected Sender
  x-api-slug: groupsidrejectedsendersref-delete
  description: Remove rejectedSender Remove a user or group from the rejectedSenders
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-delete-openapi.md
- name: Microsoft Graph API - Create Accepted Sender
  x-api-slug: groupsidacceptedsendersref-post
  description: Create acceptedSender Add a new user or group to the acceptedSender
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-post-openapi.md
- name: Microsoft Graph API - Create Rejected Sender
  x-api-slug: groupsidrejectedsendersref-post
  description: Create rejectedSender Add a new user or group to the rejectedSender
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-post-openapi.md
- name: Microsoft Graph API - List Accepted Senders
  x-api-slug: groupsidacceptedsenders-get
  description: List acceptedSenders Get a list of users or groups that are in the
    acceptedSenders list for this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsenders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsenders-get-openapi.md
- name: Microsoft Graph API - List Rejected Senders
  x-api-slug: groupsidrejectedsenders-get
  description: List rejectedSenders Get a list of users or groups that are in the
    rejectedSenders list for this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsenders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsenders-get-openapi.md
- name: Microsoft Graph API - Remove Accepted Sender
  x-api-slug: groupsidacceptedsendersref-delete
  description: Remove acceptedSender Remove a user or group from the acceptedSenders
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-delete-openapi.md
- name: Microsoft Graph API - Remove Rejected Sender
  x-api-slug: groupsidrejectedsendersref-delete
  description: Remove rejectedSender Remove a user or group from the rejectedSenders
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-delete-openapi.md
- name: Microsoft Graph API - Create Accepted Sender
  x-api-slug: groupsidacceptedsendersref-post
  description: Create acceptedSender Add a new user or group to the acceptedSender
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-post-openapi.md
- name: Microsoft Graph API - Create Rejected Sender
  x-api-slug: groupsidrejectedsendersref-post
  description: Create rejectedSender Add a new user or group to the rejectedSender
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-post-openapi.md
- name: Microsoft Graph API - List Accepted Senders
  x-api-slug: groupsidacceptedsenders-get
  description: List acceptedSenders Get a list of users or groups that are in the
    acceptedSenders list for this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsenders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsenders-get-openapi.md
- name: Microsoft Graph API - List Rejected Senders
  x-api-slug: groupsidrejectedsenders-get
  description: List rejectedSenders Get a list of users or groups that are in the
    rejectedSenders list for this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsenders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsenders-get-openapi.md
- name: Microsoft Graph API - Create Rejected Sender
  x-api-slug: groupsidrejectedsendersref-post
  description: Create rejectedSender Add a new user or group to the rejectedSender
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-post-openapi.md
- name: Microsoft Graph API - Create Accepted Sender
  x-api-slug: groupsidacceptedsendersref-post
  description: Create acceptedSender Add a new user or group to the acceptedSender
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-post-openapi.md
- name: Microsoft Graph API - Remove Rejected Sender
  x-api-slug: groupsidrejectedsendersref-delete
  description: Remove rejectedSender Remove a user or group from the rejectedSenders
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsendersref-delete-openapi.md
- name: Microsoft Graph API - Remove Accepted Sender
  x-api-slug: groupsidacceptedsendersref-delete
  description: Remove acceptedSender Remove a user or group from the acceptedSenders
    list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsendersref-delete-openapi.md
- name: Microsoft Graph API - List Rejected Senders
  x-api-slug: groupsidrejectedsenders-get
  description: List rejectedSenders Get a list of users or groups that are in the
    rejectedSenders list for this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsenders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidrejectedsenders-get-openapi.md
- name: Microsoft Graph API - List Accepted Senders
  x-api-slug: groupsidacceptedsenders-get
  description: List acceptedSenders Get a list of users or groups that are in the
    acceptedSenders list for this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsenders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-graph/groupsidacceptedsenders-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://messente.api.gallery.streamdata.io
- type: x-api-stack
  url: http://microsoft.graph.stack.network
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---