---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Send document using hash (min fn; no return)
  description: Route the document to a recipient.  The document history and status
    is updated for querying.  The API call does not return any document properties.  This
    is a <b>minimalistic function</b> for stringing with other functions
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/sendcert:
    post:
      summary: Send document using hash (min fn; no return)
      description: Route the document to a recipient.  The document history and status
        is updated for querying.  The API call does not return any document properties.  This
        is a <b>minimalistic function</b> for stringing with other functions
      operationId: EthledgerSendcertPost
      x-api-path-slug: ethledgersendcert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: recipient
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
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