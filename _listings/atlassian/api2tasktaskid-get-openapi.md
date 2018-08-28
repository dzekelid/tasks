---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get task
  description: |-
    This endpoint is used to check the status of a [long-running asynchronous task](#async).

    When the task is finished, it will contain a **result**. The result may be arbitrary JSON, its shape different for each task type. Consult the documentation of the method that created the task for more details.

    To access a task, you need to be its creator or a Jira admin. Otherwise a 403 response will be returned.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /longtask:
    get:
      summary: Get long-running tasks
      description: "Returns information about all active long-running tasks (e.g.
        space export), \nsuch as how long each task has been running and the percentage
        of each task \nthat has completed.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**:\nPermission to access the Confluence site ('Can use' global permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.LongTaskResource.getTasks_get
      x-api-path-slug: longtask-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of tasks to return per page
      - in: query
        name: start
        description: The starting index of the returned tasks
      responses:
        200:
          description: OK
      tags:
      - Long-running
      - Tasks
  /longtask/{id}:
    get:
      summary: Get long-running task
      description: "Returns information about an active long-running task (e.g. space
        export), \nsuch as how long it has been running and the percentage of the
        task that \nhas completed.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**:\nPermission to access the Confluence site ('Can use' global permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.LongTaskResource.getTask_get
      x-api-path-slug: longtaskid-get
      parameters:
      - in: path
        name: id
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Long-running
      - Task
  /api/2/task/{taskId}:
    get:
      summary: Get task
      description: |-
        This endpoint is used to check the status of a [long-running asynchronous task](#async).

        When the task is finished, it will contain a **result**. The result may be arbitrary JSON, its shape different for each task type. Consult the documentation of the method that created the task for more details.

        To access a task, you need to be its creator or a Jira admin. Otherwise a 403 response will be returned.
      operationId: com.atlassian.jira.rest.v2.task.TaskResource.getTask_get
      x-api-path-slug: api2tasktaskid-get
      parameters:
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Task
  /api/2/task/{taskId}/cancel:
    post:
      summary: Cancel task
      description: |-
        Requests that the task that corresponds to the given task id is cancelled.

        To cancel a task, you need to be its creator or a Jira admin. Otherwise a 403 response will be returned.
      operationId: com.atlassian.jira.rest.v2.task.TaskResource.cancelTask_post
      x-api-path-slug: api2tasktaskidcancel-post
      parameters:
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Cancel
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