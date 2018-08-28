swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/notify:
    post:
      summary: Notify
      description: Sends an email notification to the list of users defined in the
        request body parameters.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.notify_post
      x-api-path-slug: api2issueissueidorkeynotify-post
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue a notification is sent for
      responses:
        200:
          description: OK
      tags:
      - Notify
  /api/2/permissionscheme/{schemeId}:
    put:
      summary: Update permission scheme
      description: |-
        Updates a permission scheme. Below are some important things to note when using this resource:

        *   If a permissions list is present in the request, then it will be set in the permission scheme, overwriting _all existing_ grants.
        *   If you want to update only the name and description, then do not send a permissions list in the request.
        *   Sending an empty list will remove all permission grants from the permission scheme.

        If you want to add or delete a single permission grant instead of updating the whole list, see [Create permission grant](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-permissionscheme-schemeId-permission-post) or [Delete permission scheme entity](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-permissionscheme-schemeId-permission-permissionId-delete). See [About permission schemes and grants](https://developer.atlassian.com/cloud/jira/platform/rest/#about-permission-schemes) for more details. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.permissionscheme.PermissionSchemeResource.updatePermissionScheme_pu
      x-api-path-slug: api2permissionschemeschemeid-put
      parameters:
      - in: query
        name: expand
        description: Use expand to include additional information in the response
      - in: path
        name: schemeId
        description: The ID of the permission scheme to update (e
      responses:
        200:
          description: OK
      tags:
      - Permission
      - Scheme
  /site/{cloudId}/conversation/user/{userId}/message:
    post:
      summary: Send message to a user
      description: Send message to a user.
      operationId: UserMessagePostHandler
      x-api-path-slug: sitecloudidconversationuseruseridmessage-post
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
      - To
      - User
  /site/{cloudId}/conversation/{conversationId}/message:
    post:
      summary: Send a message to a conversation
      description: Send a message to a conversation.
      operationId: ConversationMessagePostHandler
      x-api-path-slug: sitecloudidconversationconversationidmessage-post
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
      - To
      - Conversation