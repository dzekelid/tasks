swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
  /dags/status/{dagName}/tasks/{taskId}:
    get:
      summary: Get Dags Status Tasks Taskid
      description: Get dags status tasks taskid.
      operationId: getTaskStatusUsingGET
      x-api-path-slug: dagsstatusdagnametaskstaskid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: taskId
        description: taskId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Taskid
  /dags/status/{dagName}/tasks/{taskId}/runs/{runId}:
    get:
      summary: Get Dags Status Tasks Taskid Runs Runid
      description: Get dags status tasks taskid runs runid.
      operationId: getUniqueRunTaskStatusUsingGET
      x-api-path-slug: dagsstatusdagnametaskstaskidrunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      - in: path
        name: taskId
        description: taskId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Taskid
      - Runs
      - Runid