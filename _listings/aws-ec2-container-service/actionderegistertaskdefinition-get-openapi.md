---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Deregister Task Definition
  version: 1.0.0
  description: Deregisters the specified task definition by family and revision.
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
  /?Action=StartTask:
    get:
      summary: Start Task
      description: |-
        Starts a new task from the specified task definition on the specified container
                    instance or instances.
      operationId: startTask
      x-api-path-slug: actionstarttask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to start your task
        type: string
      - in: query
        name: containerInstances
        description: The container instance IDs or full Amazon Resource Name (ARN)
          entries for the container instances on            which you would like to
          place your task
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
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=StopTask:
    get:
      summary: Stop Task
      description: Stops a running task.
      operationId: stopTask
      x-api-path-slug: actionstoptask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the task to stop
        type: string
      - in: query
        name: reason
        description: An optional message specified when a task is stopped
        type: string
      - in: query
        name: task
        description: The task ID or full Amazon Resource Name (ARN) entry of the task
          to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=DeregisterTaskDefinition:
    get:
      summary: Deregister Task Definition
      description: Deregisters the specified task definition by family and revision.
      operationId: deregisterTaskDefinition
      x-api-path-slug: actionderegistertaskdefinition-get
      parameters:
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to deregister
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=DescribeTaskDefinition:
    get:
      summary: Describe Task Definition
      description: Describes a task definition.
      operationId: describeTaskDefinition
      x-api-path-slug: actiondescribetaskdefinition-get
      parameters:
      - in: query
        name: taskDefinition
        description: The family for the latest ACTIVE revision,                family
          and revision (family:revision) for a            specific revision in the
          family, or full Amazon Resource Name (ARN) of the task definition to            describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=ListTaskDefinitionFamilies:
    get:
      summary: List Task Definition Families
      description: |-
        Returns a list of task definition families that are registered to your account
                    (which may include task definition families that no longer have any ACTIVE
                    task definition revisions).
      operationId: listTaskDefinitionFamilies
      x-api-path-slug: actionlisttaskdefinitionfamilies-get
      parameters:
      - in: query
        name: familyPrefix
        description: The familyPrefix is a string that is used to filter the results
          of                ListTaskDefinitionFamilies
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition family results returned
          by                ListTaskDefinitionFamilies in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitionFamilies
          request where maxResults was            used and the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: status
        description: The task definition family status with which to filter the                ListTaskDefinitionFamilies
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definition Families
  /?Action=ListTaskDefinitions:
    get:
      summary: List Task Definitions
      description: Returns a list of task definitions that are registered to your
        account.
      operationId: listTaskDefinitions
      x-api-path-slug: actionlisttaskdefinitions-get
      parameters:
      - in: query
        name: familyPrefix
        description: The full family name with which to filter the ListTaskDefinitions            results
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition results returned by                ListTaskDefinitions
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitions
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: sort
        description: The order in which to sort the results
        type: string
      - in: query
        name: status
        description: The task definition status with which to filter the                ListTaskDefinitions
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=RegisterTaskDefinition:
    get:
      summary: Register Task Definition
      description: |-
        Registers a new task definition from the supplied family and
                        containerDefinitions.
      operationId: registerTaskDefinition
      x-api-path-slug: actionregistertaskdefinition-get
      parameters:
      - in: query
        name: containerDefinitions
        description: A list of container definitions in JSON format that describe
          the different            containers that make up your task
        type: string
      - in: query
        name: family
        description: You must specify a family for a task definition, which allows
          you to            track multiple versions of the same task definition
        type: string
      - in: query
        name: networkMode
        description: The Docker networking mode to use for the containers in the task
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: taskRoleArn
        description: The short name or full Amazon Resource Name (ARN) of the IAM
          role that containers in this task can            assume
        type: string
      - in: query
        name: volumes
        description: A list of volume definitions in JSON format that containers in
          your task may            use
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=SubmitTaskStateChange:
    get:
      summary: Submit Task State Change
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: submitTaskStateChange
      x-api-path-slug: actionsubmittaskstatechange-get
      responses:
        200:
          description: OK
      tags:
      - Task State Change
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