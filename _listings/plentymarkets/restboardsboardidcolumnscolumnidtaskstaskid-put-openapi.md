---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Updates a task.
  description: Updates a task..
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/boards/{boardId}/columns/{columnId}/tasks:
    post:
      summary: Creates a new tasks on a specified column.
      description: Creates a new tasks on a specified column..
      operationId: postRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-post
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns/{columnId}/tasks
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      - in: path
        name: columnId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Tasks
      - "On"
      - Specified
      - Column
    get:
      summary: Lists all tasks for a given column.
      description: Lists all tasks for a given column..
      operationId: getRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: startAt
        description: Position of a task to start listing at
      - in: query
        name: tasksPerPage
        description: Number of tasks to list per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Tasksa
      - Given
      - Column
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}:
    delete:
      summary: Deletes a task.
      description: Deletes a task..
      operationId: deleteRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-delete
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Task
    get:
      summary: Gets a task by its ID.
      description: Gets a task by its id..
      operationId: getRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Task
      - By
      - Its
      - ID
    post:
      summary: Copies a specific task.
      description: Copies a specific task..
      operationId: postRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Copies
      - Specific
      - Task
    put:
      summary: Updates a task.
      description: Updates a task..
      operationId: putRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-put
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Task
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/position:
    put:
      summary: Updates the position of a task.
      description: Updates the position of a task..
      operationId: putRestBoardsBoardColumnsColumnTasksTaskPosition
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidposition-put
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: position
        description: The new position of the task
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Position
      - Of
      - Task
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references:
    post:
      summary: Creates a new reference from a given task to a contact or a ticket.
      description: Creates a new reference from a given task to a contact or a ticket..
      operationId: postRestBoardsBoardColumnsColumnTasksTaskReferences
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferences-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: referenceValue
        description: Reference type followed by foreign ID of the referenced object
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Reference
      - From
      - Given
      - Task
      - To
      - Contact
      - Ticket
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references/{referenceId}:
    delete:
      summary: Deletes a reference from a given task.
      description: Deletes a reference from a given task..
      operationId: deleteRestBoardsBoardColumnsColumnTasksTaskReferencesReference
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferencesreferenceid-delete
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: referenceId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Reference
      - From
      - Given
      - Task
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