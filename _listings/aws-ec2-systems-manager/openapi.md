swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeMaintenanceWindowExecutionTasks:
    get:
      summary: Describe Maintenance Window Execution Tasks
      description: For a given Maintenance Window execution, lists the tasks that
        were executed.
      operationId: describeMaintenanceWindowExecutionTasks
      x-api-path-slug: actiondescribemaintenancewindowexecutiontasks-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to scope down the returned tasks
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution whose task executions
          should be   retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
      - Tasks
  /?Action=DescribeMaintenanceWindowTasks:
    get:
      summary: Describe Maintenance Window Tasks
      description: Lists the tasks in a Maintenance Window.
      operationId: describeMaintenanceWindowTasks
      x-api-path-slug: actiondescribemaintenancewindowtasks-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to narrow down the scope of the returned
          tasks
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window whose tasks should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Tasks
  /?Action=RegisterTaskWithMaintenanceWindow:
    get:
      summary: Register Task With Maintenance Window
      description: Adds a new task to a Maintenance Window.
      operationId: registerTaskWithMaintenanceWindow
      x-api-path-slug: actionregistertaskwithmaintenancewindow-get
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: LoggingInfo
        description: A structure containing information about an Amazon S3 bucket
          to write instance-level logs to
        type: string
      - in: query
        name: MaxConcurrency
        description: The maximum number of targets this task can be run for in parallel
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed before this task stops being
          scheduled
        type: string
      - in: query
        name: Priority
        description: The priority of the task in the Maintenance Window, the lower
          the number the higher the   priority
        type: string
      - in: query
        name: ServiceRoleArn
        description: The role that should be assumed when executing the task
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: TaskArn
        description: The ARN of the task to execute
        type: string
      - in: query
        name: TaskParameters
        description: The parameters that should be passed to the task when it is executed
        type: string
      - in: query
        name: TaskType
        description: The type of task being registered
        type: string
      - in: query
        name: WindowId
        description: The id of the Maintenance Window the task should be added to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - TaskMaintenance
      - Window
  /?Action=DeregisterTaskFromMaintenanceWindow:
    get:
      summary: Deregister Task From Maintenance Window
      description: Removes a task from a Maintenance Window.
      operationId: deregisterTaskFromMaintenanceWindow
      x-api-path-slug: actionderegistertaskfrommaintenancewindow-get
      parameters:
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the task should be removed from
        type: string
      - in: query
        name: WindowTaskId
        description: The ID of the task to remove from the Maintenance Window
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Task
      - From
      - Maintenance
      - Window
  /?Action=DescribeMaintenanceWindowExecutionTaskInvocations:
    get:
      summary: Describe Maintenance Window Execution Task Invocations
      description: |-
        Retrieves the individual task executions (one per target) for a particular task executed
           as part of a Maintenance Window execution.
      operationId: describeMaintenanceWindowExecutionTaskInvocations
      x-api-path-slug: actiondescribemaintenancewindowexecutiontaskinvocations-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to scope down the returned task invocations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TaskId
        description: The ID of the specific task in the Maintenance Window task that
          should be   retrieved
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution the task is part of
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
      - Task
      - Invocations
  /?Action=GetMaintenanceWindowExecutionTask:
    get:
      summary: Get Maintenance Window Execution Task
      description: |-
        Retrieves the details about a specific task executed as part of a Maintenance Window
           execution.
      operationId: getMaintenanceWindowExecutionTask
      x-api-path-slug: actiongetmaintenancewindowexecutiontask-get
      parameters:
      - in: query
        name: TaskId
        description: The ID of the specific task execution in the Maintenance Window
          task that should be   retrieved
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution that includes the
          task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
      - Task