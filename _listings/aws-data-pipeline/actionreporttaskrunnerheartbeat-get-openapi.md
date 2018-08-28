---
swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 0
info:
  title: AWS Data Pipeline API Report Task Runner Heartbeat
  version: 1.0.0
  description: Task runners call ReportTaskRunnerHeartbeat every 15 minutes to indicate
    that they are operational.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PollForTask:
    get:
      summary: Poll For Task
      description: Task runners call PollForTask to receive a task to perform from
        AWS Data Pipeline.
      operationId: pollForTask
      x-api-path-slug: actionpollfortask-get
      parameters:
      - in: query
        name: hostname
        description: The public DNS name of the calling task runner
        type: string
      - in: query
        name: instanceIdentity
        description: Identity information for the EC2 instance that is hosting the
          task runner
        type: string
      - in: query
        name: workerGroup
        description: The type of task the task runner is configured to accept and
          process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=ReportTaskProgress:
    get:
      summary: Report Task Progress
      description: Task runners call ReportTaskProgress when assigned a task to acknowledge
        that it has the task.
      operationId: reportTaskProgress
      x-api-path-slug: actionreporttaskprogress-get
      parameters:
      - in: query
        name: fields
        description: Key-value pairs that define the properties of the ReportTaskProgressInput
          object
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SetTaskStatus:
    get:
      summary: Set Task Status
      description: Task runners call SetTaskStatus to notify AWS Data Pipeline that
        a task is completed and provide information about the final status.
      operationId: setTaskStatus
      x-api-path-slug: actionsettaskstatus-get
      parameters:
      - in: query
        name: errorId
        description: If an error occurred during the task, this value specifies the
          error code
        type: string
      - in: query
        name: errorMessage
        description: If an error occurred during the task, this value specifies a
          text description of the error
        type: string
      - in: query
        name: errorStackTrace
        description: If an error occurred during the task, this value specifies the
          stack trace associated with the error
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      - in: query
        name: taskStatus
        description: If FINISHED, the task successfully completed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=EvaluateExpression:
    get:
      summary: Evaluate Expression
      description: Task runners call EvaluateExpression to evaluate a string in the
        context of the specified object.
      operationId: evaluateExpression
      x-api-path-slug: actionevaluateexpression-get
      parameters:
      - in: query
        name: expression
        description: The expression to evaluate
        type: string
      - in: query
        name: objectId
        description: The ID of the object
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Expressions
  /?Action=ReportTaskRunnerHeartbeat:
    get:
      summary: Report Task Runner Heartbeat
      description: Task runners call ReportTaskRunnerHeartbeat every 15 minutes to
        indicate that they are operational.
      operationId: reportTaskRunnerHeartbeat
      x-api-path-slug: actionreporttaskrunnerheartbeat-get
      parameters:
      - in: query
        name: hostname
        description: The public DNS name of the task runner
        type: string
      - in: query
        name: taskrunnerId
        description: The ID of the task runner
        type: string
      - in: query
        name: workerGroup
        description: The type of task the task runner is configured to accept and
          process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Runner Hearbeat
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