---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Get Dags Status Tasks Runs Runid
  description: Get dags status tasks runs runid.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dags/status/{dagName}/tasks:
    get:
      summary: Get Dags Status Tasks
      description: Get dags status tasks.
      operationId: getAllDagTasksUsingGET
      x-api-path-slug: dagsstatusdagnametasks-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: query
        name: end_time
        description: end_time
      - in: query
        name: start_time
        description: start_time
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
  /dags/status/{dagName}/tasks/runs/{runId}:
    get:
      summary: Get Dags Status Tasks Runs Runid
      description: Get dags status tasks runs runid.
      operationId: getTaskStatusByRunIdUsingGET
      x-api-path-slug: dagsstatusdagnametasksrunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Runs
      - Runid
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