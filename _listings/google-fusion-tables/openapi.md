swagger: "2.0"
x-collection-name: Google Fusion Tables
x-complete: 1
info:
  title: Fusion Tables
  description: api-for-working-with-fusion-tables-data-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /fusiontables/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tables/{tableId}/tasks:
    get:
      summary: Get Tasks
      description: Retrieves a list of tasks.
      operationId: fusiontables.task.list
      x-api-path-slug: tablestableidtasks-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of tasks to return
      - in: query
        name: pageToken
        description: Continuation token specifying which result page to return
      - in: query
        name: startIndex
        description: Index of the first result returned in the current page
      - in: path
        name: tableId
        description: Table whose tasks are being listed
      responses:
        200:
          description: OK
      tags:
      - Task
  /tables/{tableId}/tasks/{taskId}:
    delete:
      summary: Delete Task
      description: Deletes a specific task by its ID, unless that task has already
        started running.
      operationId: fusiontables.task.delete
      x-api-path-slug: tablestableidtaskstaskid-delete
      parameters:
      - in: path
        name: tableId
        description: Table from which the task is being deleted
      - in: path
        name: taskId
        description: The identifier of the task to delete
      responses:
        200:
          description: OK
      tags:
      - Task
    get:
      summary: Get Task
      description: Retrieves a specific task by its ID.
      operationId: fusiontables.task.get
      x-api-path-slug: tablestableidtaskstaskid-get
      parameters:
      - in: path
        name: tableId
        description: Table to which the task belongs
      - in: path
        name: taskId
        description: The identifier of the task to get
      responses:
        200:
          description: OK
      tags:
      - Task