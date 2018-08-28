---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Save or Updates a Property ToDo and and its tasks
  version: 1.0.0
  description: Save or updates a property todo and and its tasks.
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
  /api/todo/teamtodos:
    get:
      summary: Get the list of completed tasks of a Todo
      description: Get the list of completed tasks of a todo.
      operationId: DefaultToDo_TeamTodosBybranchId
      x-api-path-slug: apitodoteamtodos-get
      parameters:
      - in: query
        name: branchId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
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
  /api/todo/canceltasks:
    put:
      summary: Cancel a single or multiple tasks from a to-do bucket
      description: Cancel a single or multiple tasks from a to-do bucket.
      operationId: DefaultToDo_CancelTasksBycancelTasksCommandData
      x-api-path-slug: apitodocanceltasks-put
      parameters:
      - in: body
        name: cancelTasksCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Single
      - Multiple
      - Tasks
      - From
      - To-do
      - Bucket
  /api/todo/reassigntodotasks:
    put:
      summary: Reassign a list of tasks to different negotiator(s)
      description: Reassign a list of tasks to different negotiator(s).
      operationId: DefaultToDo_ReassignTodoTasksByreassignTasksCommandData
      x-api-path-slug: apitodoreassigntodotasks-put
      parameters:
      - in: body
        name: reassignTasksCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reassign
      - List
      - Of
      - Tasks
      - To
      - Different
      - Negotiator(s)
  /api/todo/gettodosbyid:
    get:
      summary: Return list of tasks, corresponding to task ids passed in.
      description: Return list of tasks, corresponding to task ids passed in..
      operationId: DefaultToDo_GetTodosByIdByids
      x-api-path-slug: apitodogettodosbyid-get
      parameters:
      - in: query
        name: ids
        description: List of task ids
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Tasks
      - ""
      - Corresponding
      - To
      - Task
      - Ids
      - Passed
      - In
  /api/todo/event/savetodo:
    post:
      summary: Save or Updates a Event ToDo and and its tasks
      description: Save or updates a event todo and and its tasks.
      operationId: EventToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodoeventsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - S
      - Event
      - ToDo
      - And
      - Its
      - Tasks
  /api/todo/event/addtasks:
    put:
      summary: Add tasks to a Event ToDo
      description: Add tasks to a event todo.
      operationId: EventToDo_AddTasksByaddEventTasksCommandDataContract
      x-api-path-slug: apitodoeventaddtasks-put
      parameters:
      - in: body
        name: addEventTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - To
      - Event
      - ToDo
  /api/todo/group/savetodo:
    post:
      summary: Saves or Updates a Group ToDo and its tasks
      description: Saves or updates a group todo and its tasks.
      operationId: GroupToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodogroupsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - S
      - Group
      - ToDo
      - Its
      - Tasks
  /api/list/todotasks:
    post:
      summary: Get list of todos tasks.
      description: Get list of todos tasks..
      operationId: List_TodoTasksByfilterBypageSizeBypageNumber
      x-api-path-slug: apilisttodotasks-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Todos
      - Tasks
  /api/todo/property/savetodo:
    post:
      summary: Save or Updates a Property ToDo and and its tasks
      description: Save or updates a property todo and and its tasks.
      operationId: PropertyToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodopropertysavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - S
      - Property
      - ToDo
      - And
      - Its
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