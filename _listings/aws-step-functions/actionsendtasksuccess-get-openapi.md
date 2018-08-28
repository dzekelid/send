---
swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 0
info:
  title: AWS Step Functions API Send Task Success
  version: 1.0.0
  description: Used by workers to report that the task identified by the taskToken
    completed successfully.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SendTaskFailure:
    get:
      summary: Send Task Failure
      description: Used by workers to report that the task identified by the taskToken
        failed.
      operationId: sendTaskFailure
      x-api-path-slug: actionsendtaskfailure-get
      parameters:
      - in: query
        name: cause
        description: A more detailed explanation of the cause of the failure
        type: string
      - in: query
        name: error
        description: An arbitrary error code that identifies the cause of the failure
        type: string
      - in: query
        name: taskToken
        description: The token that represents this task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SendTaskHeartbeat:
    get:
      summary: Send Task Heartbeat
      description: "Used by workers to report to the service that the task represented
        by the specified taskToken \n    is still making progress."
      operationId: sendTaskHeartbeat
      x-api-path-slug: actionsendtaskheartbeat-get
      parameters:
      - in: query
        name: taskToken
        description: The token that represents this task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SendTaskSuccess:
    get:
      summary: Send Task Success
      description: Used by workers to report that the task identified by the taskToken
        completed successfully.
      operationId: sendTaskSuccess
      x-api-path-slug: actionsendtasksuccess-get
      parameters:
      - in: query
        name: output
        description: The JSON output of the task
        type: string
      - in: query
        name: taskToken
        description: The token that represents this task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
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