---
name: ChainGenie
x-slug: chaingenie
description: ChainGenie provides a plug and play platform that helps you connect your
  existing (or create new) applications to DLTs for lodging and workflow management
  using a simple easy to use user interface. ChainGenie is a platform to create blockchain
  apps that provide speed-to-market for companies looking to launch faster, rather
  than reinvent the wheel. Write your applications to run on popular Blockchain networks
  like Ethereum, Bitcoin Blockchain etc with great ease when you require to validate
  credentials or make your existing traditional applications use the power of DLT
  and blockchain overnight!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
x-kinRank: "7"
x-alexaRank: ""
tags: Send
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/chaingenie/apis.md
specificationVersion: "0.14"
apis:
- name: ChainGenie = DLT + Blockchain + Magic - Send document using hash (min fn;
    no return)
  x-api-slug: ethledgersendcert-post
  description: Route the document to a recipient.  The document history and status
    is updated for querying.  The API call does not return any document properties.  This
    is a <b>minimalistic function</b> for stringing with other functions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/chaingenie/ethledgersendcert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/chaingenie/ethledgersendcert-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Send document
  x-api-slug: ethledgersendforsign-post
  description: Route the document for signature.  The document history and status
    is updated for querying.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/chaingenie/ethledgersendforsign-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/send/master/_listings/chaingenie/ethledgersendforsign-post-openapi.md
x-common:
- type: x-github
  url: https://github.com/ChainGenie
- type: x-website
  url: http://chaingenie.com
- type: x-api-gallery
  url: http://broadleaf.commerce.api.gallery.streamdata.io
- type: x-twitter
  url: https://twitter.com/ChainGenie
- type: x-website
  url: http://api.chaingenie.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---