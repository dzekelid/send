---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get a list of the supported sending methods for a correspondence (ie
    all of the types required by each document in each envelope)
  version: 1.0.0
  description: Get a list of the supported sending methods for a correspondence (ie
    all of the types required by each document in each envelope).
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/digitalsignature/signable/remind/{eventId}:
    get:
      summary: Send a reminder for an Envelope
      description: Send a reminder for an envelope.
      operationId: DigitalSignature_RemindByeventId
      x-api-path-slug: apidigitalsignaturesignableremindeventid-get
      parameters:
      - in: path
        name: eventId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Send
      - Reminderan
      - Envelope
  /api/group/{id}/sendemail:
    post:
      summary: To send an adhoc email to a group
      description: To send an adhoc email to a group.
      operationId: Group_SendEmailByidByemailDataContract
      x-api-path-slug: apigroupidsendemail-post
      parameters:
      - in: body
        name: emailDataContract
        description: Details of the email to send
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Email
      - To
      - Group
  /api/group/{id}/sendsms:
    post:
      summary: To send an adhoc sms to a group
      description: To send an adhoc sms to a group.
      operationId: Group_SendSMSByidBysmsDataContract
      x-api-path-slug: apigroupidsendsms-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: smsDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Sms
      - To
      - Group
  /api/role/{id}/boardrequest:
    post:
      summary: To send an board request email to a external provider
      description: To send an board request email to a external provider.
      operationId: Role_BoardRequestByidByupdateBoardRequestDataContract
      x-api-path-slug: apiroleidboardrequest-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updateBoardRequestDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Board
      - Request
      - Email
      - To
      - External
      - Provider
  /api/admin/system/sendNotificationToAllUsersInAgency:
    post:
      summary: Send a live notification to all active users in an agency
      description: Send a live notification to all active users in an agency.
      operationId: System_SendNotificationToAgencyUsersByagencyIdBysendNotification
      x-api-path-slug: apiadminsystemsendnotificationtoallusersinagency-post
      parameters:
      - in: query
        name: agencyId
        description: The agency identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendNotification
        description: The send notification
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Live
      - Notification
      - To
      - ""
      - Active
      - Users
      - In
      - Agency
  /api/documentgeneration/singlepropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same property role.
      operationId: DocumentGeneration_SendPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglepropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Property
      - Role
  /api/documentgeneration/singlelettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same letting property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same letting property role.
      operationId: DocumentGeneration_SendLettingsPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglelettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Letting
      - Property
      - Role
  /api/documentgeneration/selectedpropertiesmatch:
    post:
      summary: Generates a correspondence to a single applicant, sending them user
        selected property roles
      description: Generates a correspondence to a single applicant, sending them
        user selected property roles.
      operationId: DocumentGeneration_SendSelectedPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedpropertiesmatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/selectedlettingspropertiesmatch:
    post:
      summary: Generates a correspondence to a single letting applicant, sending them
        user selected property roles
      description: Generates a correspondence to a single letting applicant, sending
        them user selected property roles.
      operationId: DocumentGeneration_SendSelectedLettingsPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedlettingspropertiesmatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Letting
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/multipropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them a filtered
        set of the matching property roles
      description: Generates a correspondence to multiple applicants, sending them
        a filtered set of the matching property roles.
      operationId: DocumentGeneration_SendAutoMatchedPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultipropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Property
      - Roles
  /api/documentgeneration/multilettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles
      description: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles.
      operationId: DocumentGeneration_SendAutoMatchedLettingsPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultilettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Letting
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Letting
      - Property
      - Roles
  /api/documentgeneration/vendorreport:
    post:
      summary: Generates a correspondence to a single group, sending them a single
        report for multiple properties
      description: Generates a correspondence to a single group, sending them a single
        report for multiple properties.
      operationId: DocumentGeneration_SendVendorReportBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvendorreport-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Group
      - ""
      - Sending
      - Them
      - Single
      - Reportmultiple
      - Properties
  /api/documentgeneration/packsupportedsendmethods/{packid}:
    get:
      summary: Get a list of the supported sending methods for a correspondence (ie
        all of the types required by each document in each envelope)
      description: Get a list of the supported sending methods for a correspondence
        (ie all of the types required by each document in each envelope).
      operationId: DocumentGeneration_PackSupportedSendMethodsBypackid
      x-api-path-slug: apidocumentgenerationpacksupportedsendmethodspackid-get
      parameters:
      - in: path
        name: packid
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Supported
      - Sending
      - Methodsa
      - Correspondence
      - (ie
      - ""
      - Of
      - Types
      - Required
      - By
      - Each
      - Document
      - In
      - Each
      - Envelope)
  /api/coreplatformstate/sendpendingalerts:
    post:
      summary: Sends alerts for all current platform issues.
      description: Sends alerts for all current platform issues..
      operationId: CorePlatformState_SendPendingAlerts
      x-api-path-slug: apicoreplatformstatesendpendingalerts-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Alerts
      - Current
      - Platform
      - Issues
  /api/documentgeneration/viewing/feedback:
    post:
      summary: Sends viewing feedback to Owner / Landlord
      description: Sends viewing feedback to owner / landlord.
      operationId: DocumentGeneration_ViewingFeedbackBygeneratePackDataContract
      x-api-path-slug: apidocumentgenerationviewingfeedback-post
      parameters:
      - in: body
        name: generatePackDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Viewing
      - Feedback
      - To
      - Owner
      - ""
      - ""
      - Landlord
  /api/job/SendSystemEmail:
    post:
      summary: Sends a basic email to any specified party.
      description: Sends a basic email to any specified party..
      operationId: Job_SendSystemEmailBysendSystemEmail
      x-api-path-slug: apijobsendsystememail-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendSystemEmail
        description: The send system email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Basic
      - Email
      - To
      - Any
      - Specified
      - Party
  /api/people/sendnotification:
    post:
      summary: Sends a user notification to the specified user
      description: Sends a user notification to the specified user.
      operationId: People_SendNotificationBysendNotificationToPerson
      x-api-path-slug: apipeoplesendnotification-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendNotificationToPerson
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - User
      - Notification
      - To
      - Specified
      - User
  /api/admin/system/sendliveportalupdatemessage:
    post:
      summary: "Sends a message to the LivePortalJobHandler that says \r\nthe specified
        property marketing role has changed"
      description: "Sends a message to the liveportaljobhandler that says \r\nthe
        specified property marketing role has changed."
      operationId: System_SendLivePortalUpdateMessageBypropertyMarketingRoleId
      x-api-path-slug: apiadminsystemsendliveportalupdatemessage-post
      parameters:
      - in: query
        name: propertyMarketingRoleId
        description: The property marketing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Message
      - To
      - LivePortalJobHandler
      - That
      - Says
      - The
      - Specified
      - Property
      - Marketing
      - Role
      - Has
      - Changed
  /api/twitter/directmessage:
    post:
      summary: Sends a direct message to a screen name
      description: Sends a direct message to a screen name.
      operationId: Twitter_TwitterDirectMessageBydirectMessage
      x-api-path-slug: apitwitterdirectmessage-post
      parameters:
      - in: body
        name: directMessage
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Direct
      - Message
      - To
      - Screen
      - Name
  /api/twitter/tweet:
    post:
      summary: Sends a direct message to a screen name
      description: Sends a direct message to a screen name.
      operationId: Twitter_TwitterDirectMessageBytweet
      x-api-path-slug: apitwittertweet-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: tweet
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Direct
      - Message
      - To
      - Screen
      - Name
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