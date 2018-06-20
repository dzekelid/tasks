---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM DELETE for Task
  description: Delete task information
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /task:
    get:
      summary: GET for Task
      description: Returns all tasks from the system
      operationId: getTaskCollection
      x-api-path-slug: task-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
    post:
      summary: POST for Task
      description: Add task into the system
      operationId: createTaskEntity
      x-api-path-slug: task-post
      parameters:
      - in: body
        name: body
        description: Add task into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /task/count:
    get:
      summary: COUNT for Task
      description: Count all tasks from the system
      operationId: getTaskCountCollection
      x-api-path-slug: taskcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - Count
  /task/describe:
    get:
      summary: DESCRIBE for Task
      description: Returns describe for tasks
      operationId: getTaskDescribe
      x-api-path-slug: taskdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - Describe
  /task/{task_id}:
    delete:
      summary: DELETE for Task
      description: Delete task information
      operationId: deleteTaskEntity
      x-api-path-slug: tasktask-id-delete
      parameters:
      - in: path
        name: task_id
        description: Task Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
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