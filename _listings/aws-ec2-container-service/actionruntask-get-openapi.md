---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Run Task
  version: 1.0.0
  description: Starts a new task using the specified task definition.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTasks:
    get:
      summary: Describe Tasks
      description: Describes a specified task or tasks.
      operationId: describeTasks
      x-api-path-slug: actiondescribetasks-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the task to describe
        type: string
      - in: query
        name: tasks
        description: A space-separated list of task IDs or full Amazon Resource Name
          (ARN) entries
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=ListTasks:
    get:
      summary: List Tasks
      description: Returns a list of tasks for a specified cluster.
      operationId: listTasks
      x-api-path-slug: actionlisttasks-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the tasks to list
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          of the container instance with which to            filter the ListTasks
          results
        type: string
      - in: query
        name: desiredStatus
        description: The task desired status with which to filter the ListTasks results
        type: string
      - in: query
        name: family
        description: The name of the family with which to filter the ListTasks results
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task results returned by ListTasks in paginated            output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTasks
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      - in: query
        name: serviceName
        description: The name of the service with which to filter the ListTasks results
        type: string
      - in: query
        name: startedBy
        description: The startedBy value with which to filter the task results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=RunTask:
    get:
      summary: Run Task
      description: Starts a new task using the specified task definition.
      operationId: runTask
      x-api-path-slug: actionruntask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to run your task
        type: string
      - in: query
        name: count
        description: The number of instantiations of the specified task to place on
          your            cluster
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: placementStrategy
        description: The placement strategy objects to use for the task
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run
        type: string
      responses:
        200:
          description: OK
      tags:
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