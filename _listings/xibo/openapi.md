swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/action/command:
    post:
      summary: Send Command
      description: Send a predefined command to this Group of Displays
      operationId: displayGroupActionCommand
      x-api-path-slug: displaygroupdisplaygroupidactioncommand-post
      parameters:
      - in: formData
        name: commandId
        description: The Command Id
      - in: path
        name: displayGroupId
        description: The display group id
      responses:
        200:
          description: OK
      tags:
      - Send
      - Command