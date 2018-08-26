---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark Account-level
  description: postmark-makes-sending-and-receiving-email-incredibly-easy--the-accountlevel-api-allows-users-toconfigure-all-servers-domains-and-sender-signatures-associated-with-an-account-
  version: 0.9.0
host: api.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /senders:
    get:
      summary: List Sender Signatures
      description: List sender signatures.
      operationId: listSenderSignatures
      x-api-path-slug: senders-get
      parameters:
      - in: query
        name: count
        description: Number of records to return per request
      - in: query
        name: offset
        description: Number of records to skip
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
    post:
      summary: Create a Sender Signature
      description: Create a sender signature.
      operationId: createSenderSignature
      x-api-path-slug: senders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
  /senders/{signatureid}:
    delete:
      summary: Delete a Sender Signature
      description: Delete a sender signature.
      operationId: deleteSenderSignature
      x-api-path-slug: senderssignatureid-delete
      parameters:
      - in: path
        name: signatureid
        description: The ID for the Sender Signature that should be deleted by the
          request
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
      - Signatureid
    get:
      summary: Get a Sender Signature
      description: Get a sender signature.
      operationId: getSenderSignature
      x-api-path-slug: senderssignatureid-get
      parameters:
      - in: path
        name: signatureid
        description: The ID for the Sender Signature that should be retrieved
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
      - Signatureid
    put:
      summary: Update a Sender Signature
      description: Update a sender signature.
      operationId: editSenderSignature
      x-api-path-slug: senderssignatureid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: signatureid
        description: The ID for the Sender Signature that should be modified by the
          request
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
      - Signatureid
  /senders/{signatureid}/requestnewdkim:
    post:
      summary: Request a new DKIM Key
      description: "Requests a new DKIM key to be created. Until the DNS entries are
        confirmed, \nthe new values will be in the `DKIMPendingHost` and `DKIMPendingTextValue`
        fields. \nAfter the new DKIM value is verified in DNS, the pending values
        will migrate to \n`DKIMTextValue` and `DKIMPendingTextValue` and Postmark
        will begin to sign emails \nwith the new DKIM key."
      operationId: requestNewDKIMKeyForSenderSignature
      x-api-path-slug: senderssignatureidrequestnewdkim-post
      parameters:
      - in: path
        name: signatureid
        description: The ID for the Sender Signature for which a new DKIM Key should
          be generated
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
      - Signatureid
      - Requestnewdkim
  /senders/{signatureid}/resend:
    post:
      summary: Resend Signature Confirmation Email
      description: Resend signature confirmation email.
      operationId: resendSenderSignatureConfirmationEmail
      x-api-path-slug: senderssignatureidresend-post
      parameters:
      - in: path
        name: signatureid
        description: The ID for the Sender Signature that should have its confirmation
          email resent
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
      - Signatureid
      - Resend
  /senders/{signatureid}/verifyspf:
    post:
      summary: Request DNS Verification for SPF
      description: Request dns verification for spf.
      operationId: requestSPFVerificationForSenderSignature
      x-api-path-slug: senderssignatureidverifyspf-post
      parameters:
      - in: path
        name: signatureid
        description: The ID for the Sender Signature for which SPF DNS records should
          be verified
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Senders
      - Signatureid
      - Verifyspf
---