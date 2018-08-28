---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Add task to a Group ToDo
  version: 1.0.0
  description: Add task to a group todo.
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
  /api/todo/property/addtasks:
    put:
      summary: Add tasks to a Property ToDo
      description: Add tasks to a property todo.
      operationId: PropertyToDo_AddTasksByaddPropertyTasksCommandDataContract
      x-api-path-slug: apitodopropertyaddtasks-put
      parameters:
      - in: body
        name: addPropertyTasksCommandDataContract
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
      - Property
      - ToDo
  /api/todo/group/getupcomingtask:
    get:
      summary: Get the todo and latest task for a group
      description: Get the todo and latest task for a group.
      operationId: GroupToDo_GetUpComingTaskBygroupId
      x-api-path-slug: apitodogroupgetupcomingtask-get
      parameters:
      - in: query
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Todo
      - Latest
      - Taska
      - Group
  /api/todo/event/task/{eventId}:
    get:
      summary: Gets all tasks for a particular event / appointment
      description: Gets all tasks for a particular event / appointment.
      operationId: EventToDo_EventTasksByeventIdBypageSizeBypageNumber
      x-api-path-slug: apitodoeventtaskeventid-get
      parameters:
      - in: path
        name: eventId
        description: Id of event or appointment
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tasksa
      - Particular
      - Event
      - ""
      - ""
      - Appointment
  /api/todo/getclaimedtask:
    get:
      summary: Get Claimed Task by id
      description: Get claimed task by id.
      operationId: DefaultToDo_GetClaimedTaskBytaskId
      x-api-path-slug: apitodogetclaimedtask-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Claimed
      - Task
      - By
      - Id
  /api/todo/updatetaskrecurrence:
    put:
      summary: Update the date of recurrence of a task
      description: Update the date of recurrence of a task.
      operationId: DefaultToDo_UpdateTaskRecurrenceBytaskRecurrence
      x-api-path-slug: apitodoupdatetaskrecurrence-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: taskRecurrence
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Recurrence
      - Of
      - Task
  /api/todo/claimtask:
    put:
      summary: Sets the claiming negotiator for the task
      description: Sets the claiming negotiator for the task.
      operationId: DefaultToDo_ClaimTaskByclaimTask
      x-api-path-slug: apitodoclaimtask-put
      parameters:
      - in: body
        name: claimTask
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Claiming
      - Negotiatorthe
      - Task
  /api/todo/releasetask:
    put:
      summary: Release task
      description: Release task.
      operationId: DefaultToDo_ReleaseTaskBytaskId
      x-api-path-slug: apitodoreleasetask-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Release
      - Task
  /api/todo/snoozetask:
    put:
      summary: Snooze task
      description: Snooze task.
      operationId: DefaultToDo_SnoozeTaskBysnoozeTask
      x-api-path-slug: apitodosnoozetask-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: snoozeTask
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Snooze
      - Task
  /api/todo/addtasknote:
    post:
      summary: Add note for a task
      description: Add note for a task.
      operationId: DefaultToDo_AddTaskNoteBynote
      x-api-path-slug: apitodoaddtasknote-post
      parameters:
      - in: body
        name: note
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Notea
      - Task
  /api/todo/gettasknotes/{id}:
    get:
      summary: Get notes for a task
      description: Get notes for a task.
      operationId: DefaultToDo_GetTaskNotesByid
      x-api-path-slug: apitodogettasknotesid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Notesa
      - Task
  /api/todo/canceltask:
    put:
      summary: Cancel the Task. Used for cancelling the Lead Requests.
      description: Cancel the task. used for cancelling the lead requests..
      operationId: DefaultToDo_CancelTaskBycancelTask
      x-api-path-slug: apitodocanceltask-put
      parameters:
      - in: body
        name: cancelTask
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
      - Task
      - ""
      - Usedcancelling
      - Lead
      - Requests
  /api/todo/cancelleadandtask:
    put:
      summary: Cancel the Task. Used for cancelling the Lead Requests.
      description: Cancel the task. used for cancelling the lead requests..
      operationId: DefaultToDo_CancelLeadAndTaskBycancelLead
      x-api-path-slug: apitodocancelleadandtask-put
      parameters:
      - in: body
        name: cancelLead
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
      - Task
      - ""
      - Usedcancelling
      - Lead
      - Requests
  /api/todo/assigntasktonegotiator:
    put:
      summary: Assign a task to a negotiator by its Id.
      description: Assign a task to a negotiator by its id..
      operationId: DefaultToDo_AssignTaskToNegotiatorBytaskIdBynegotiatorId
      x-api-path-slug: apitodoassigntasktonegotiator-put
      parameters:
      - in: query
        name: negotiatorId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Task
      - To
      - Negotiator
      - By
      - Its
      - Id
  /api/todo/event/task/duedate:
    post:
      summary: Updates the due date of an event task
      description: Updates the due date of an event task.
      operationId: EventToDo_UpdateTaskDueDateBycommandDataContract
      x-api-path-slug: apitodoeventtaskduedate-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Due
      - Date
      - Of
      - Event
      - Task
  /api/todo/general/taskprofile:
    get:
      summary: Get the profile infos for a task
      description: Get the profile infos for a task.
      operationId: GeneralToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodogeneraltaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Task
  /api/todo/group/addtasks:
    put:
      summary: Add task to a Group ToDo
      description: Add task to a group todo.
      operationId: GroupToDo_AddTasksByaddTasksCommandDataContract
      x-api-path-slug: apitodogroupaddtasks-put
      parameters:
      - in: body
        name: addTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Task
      - To
      - Group
      - ToDo
  /api/todo/group/taskprofile:
    get:
      summary: Get the profile infos for a task
      description: Get the profile infos for a task.
      operationId: GroupToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodogrouptaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Task
  /api/inboundlead/{todoTaskLeadId}/setleadgroup/{groupId}:
    put:
      summary: Endpoint to update group on inbound lead task
      description: Endpoint to update group on inbound lead task.
      operationId: InboundLead_SetLeadGroupBytodoTaskLeadIdBygroupId
      x-api-path-slug: apiinboundleadtodotaskleadidsetleadgroupgroupid-put
      parameters:
      - in: path
        name: groupId
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: todoTaskLeadId
        description: Todos Task Id
      responses:
        200:
          description: OK
      tags:
      - Endpoint
      - To
      - Update
      - Group
      - "On"
      - Inbound
      - Lead
      - Task
  /api/list/todotasks/filters/{id}:
    delete:
      summary: Marks Todos task List Filter as deleted
      description: Marks todos task list filter as deleted.
      operationId: List_DeleteTodoTaskListFilterByid
      x-api-path-slug: apilisttodotasksfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todos
      - Task
      - List
      - Filter
      - As
      - Deleted
  /api/todo/property/taskprofile:
    get:
      summary: Get the profile infos for a propery task
      description: Get the profile infos for a propery task.
      operationId: PropertyToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodopropertytaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Propery
      - Task
  /api/branch/updatescheduledtaskstatus/{id}:
    post:
      summary: Update SystemStatus of ScheduledTask to Active, Inactive, Deleted or
        Archived.
      description: Update systemstatus of scheduledtask to active, inactive, deleted
        or archived..
      operationId: Branch_UpdateScheduledTaskStatusByidBysystemStatus
      x-api-path-slug: apibranchupdatescheduledtaskstatusid-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: systemStatus
      responses:
        200:
          description: OK
      tags:
      - SystemStatus
      - Of
      - ScheduledTask
      - To
      - Active
      - ""
      - Inactive
      - ""
      - D
      - Archived
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