---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 0
info:
  title: Google Tasks API Get Lists Task List Tasks
  description: Returns all tasks in the specified task list.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{tasklist}/tasks:
    get:
      summary: Get Lists Task List Tasks
      description: Returns all tasks in the specified task list.
      operationId: tasks.tasks.list
      x-api-path-slug: liststasklisttasks-get
      parameters:
      - in: query
        name: completedMax
        description: Upper bound for a tasks completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: completedMin
        description: Lower bound for a tasks completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: dueMax
        description: Upper bound for a tasks due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: dueMin
        description: Lower bound for a tasks due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      - in: query
        name: showCompleted
        description: Flag indicating whether completed tasks are returned in the result
      - in: query
        name: showDeleted
        description: Flag indicating whether deleted tasks are returned in the result
      - in: query
        name: showHidden
        description: Flag indicating whether hidden tasks are returned in the result
      - in: path
        name: tasklist
        description: Task list identifier
      - in: query
        name: updatedMin
        description: Lower bound for a tasks last modification time (as a RFC 3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
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