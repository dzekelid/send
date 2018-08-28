swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /nxtportdocument/{blnumber}/ag/{agent}:
    get:
      summary: Returns the file with corresponding blnumbers and senderID.
      description: Returns the file with corresponding blnumbers and senderid..
      operationId: NxtportdocumentByBlnumberAgByAgentGet
      x-api-path-slug: nxtportdocumentblnumberagagent-get
      parameters:
      - in: path
        name: agent
        description: agent
      - in: path
        name: blnumber
        description: blnumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - File
      - Corresponding
      - Blnumbers
      - SenderID