---
name: Microsoft Office 365
x-slug: microsoft-office-365
description: Integrate Office 365 REST APIs powered by Microsoft Graph into your own
  app to connect to files, calendars, mail and more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Send
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-office-365/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Office 365 - Add Messages Event Send
  x-api-slug: messagesevent-idsend-post
  description: You can send an existing email that has the IsDraft property...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Spreadsheets, Documents, Stack Network, Stack, Productivity, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-office-365/messagesevent-idsend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-office-365/messagesevent-idsend-post-openapi.md
- name: Microsoft Office 365 - Parameters Messages Event Send
  x-api-slug: messagesevent-idsend-parameters
  description: Parameters messages event  send
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Spreadsheets, Documents, Stack Network, Stack, Productivity, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-office-365/messagesevent-idsend-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/microsoft-office-365/messagesevent-idsend-parameters-openapi.md
x-common:
- type: x-api-gallery
  url: http://microsoft.graph.api.gallery.streamdata.io
- type: x-api-stack
  url: http://microsoft.office.365.stack.network
- type: x-developer
  url: http://dev.office.com
- type: x-github
  url: https://github.com/OfficeDev
- type: x-twitter
  url: https://twitter.com/OfficeDev
- type: x-website
  url: http://office.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---