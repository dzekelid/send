swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /callback:
    post:
      summary: Sends a callback message
      description: |-
        Upon the receipt of an event, send a response in an async way to the event framework of Manufacturing Network.

        In the callback message, be sure to include the event ID. Add other information as appropriate.
      operationId: upon-the-receipt-of-an-event-send-a-response-in-an-async-way-to-the-event-framework-of-manufacturing
      x-api-path-slug: callback-post
      parameters:
      - in: body
        name: Callback
        description: A callback message
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Sends
      - Callback
      - Message