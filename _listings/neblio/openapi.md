swagger: "2.0"
x-collection-name: Neblio
x-complete: 1
info:
  title: Neblio REST API Suite
  description: apis-for-interacting-with-ntp1-tokens--the-neblio-blockchain
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ntp1/sendtoken:
    post:
      summary: Builds a transaction that sends an NTP1 Token
      description: Builds an unsigned raw transaction that sends an NTP1 token on
        the Neblio blockchain.
      operationId: sendToken
      x-api-path-slug: ntp1sendtoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be sent
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Sends
      - NTP1
      - Token
  /testnet/ntp1/sendtoken:
    post:
      summary: Builds a transaction that sends an NTP1 Token
      description: Builds an unsigned raw transaction that sends an NTP1 token on
        the Neblio blockchain.
      operationId: testnet_sendToken
      x-api-path-slug: testnetntp1sendtoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be sent
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Sends
      - NTP1
      - Token