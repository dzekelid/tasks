---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get the list of completed tasks of a Todo
  version: 1.0.0
  description: Get the list of completed tasks of a todo.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/activetasks:
    get:
      summary: Get the list of active tasks of a Todo
      description: Get the list of active tasks of a todo.
      operationId: DefaultToDo_ActiveTasksBytoDoIdByignoreDueDateBypageSizeBypageNumber
      x-api-path-slug: apitodoactivetasks-get
      parameters:
      - in: query
        name: ignoreDueDate
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Active
      - Tasks
      - Of
      - Todo
  /api/todo/completedtasks:
    get:
      summary: Get the list of completed tasks of a Todo
      description: Get the list of completed tasks of a todo.
      operationId: DefaultToDo_CompletedTasksBytoDoId
      x-api-path-slug: apitodocompletedtasks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Completed
      - Tasks
      - Of
      - Todo
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