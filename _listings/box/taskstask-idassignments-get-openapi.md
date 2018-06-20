---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Assignments
  description: Retrieves all of the assignments for a given task.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{FILE_ID}/tasks:
    get:
      summary: Get File's Tasks
      description: Retrieves all of the tasks for given file.
      operationId: getFileTasks
      x-api-path-slug: filesfile-idtasks-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FILE_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Tasks
  /tasks:
    post:
      summary: Create Task
      description: Used to create a single task for single user on a single file.
      operationId: createTask
      x-api-path-slug: tasks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
  /tasks/{TASK_ID}:
    get:
      summary: Get Task
      description: Fetches a specific task.
      operationId: getTask
      x-api-path-slug: taskstask-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: TASK_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
      - Task
    put:
      summary: Update Task
      description: Updates a specific task.
      operationId: updateTask
      x-api-path-slug: taskstask-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: TASK_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
      - Task
    delete:
      summary: Delete Task
      description: Permanently deletes a specific task.
      operationId: deleteTask
      x-api-path-slug: taskstask-id-delete
      parameters:
      - in: path
        name: TASK_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
      - Task
  /tasks/{TASK_ID}/assignments:
    get:
      summary: Get Assignments
      description: Retrieves all of the assignments for a given task.
      operationId: getTaskAssignments
      x-api-path-slug: taskstask-idassignments-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: TASK_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
      - Task
      - ""
      - Assignments
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