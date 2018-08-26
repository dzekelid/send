---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SignalResource:
    get:
      summary: Signal Resource
      description: Sends a signal to the specified resource with a success or failure
        status.
      operationId: signalResource
      x-api-path-slug: actionsignalresource-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical ID of the resource that you want to signal
        type: string
      - in: query
        name: StackName
        description: The stack name or unique stack ID that includes the resource
          that you want to signal
        type: string
      - in: query
        name: Status
        description: The status of the signal, which is either success or failure
        type: string
      - in: query
        name: UniqueId
        description: A unique ID of the signal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signal Resources
---