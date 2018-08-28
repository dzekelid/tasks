---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get long-running tasks
  description: "Returns information about all active long-running tasks (e.g. space
    export), \nsuch as how long each task has been running and the percentage of each
    task \nthat has completed.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**:\nPermission to access the Confluence site ('Can use' global permission)."
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