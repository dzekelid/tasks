---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 0
info:
  title: AWS Database Migration Service API Stop Replication Task
  version: 1.0.0
  description: Stops the replication task.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateReplicationTask:
    get:
      summary: Create Replication Task
      description: Creates a replication task using the specified parameters.
      operationId: createReplicationTask
      x-api-path-slug: actioncreatereplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: MigrationType
        description: The migration type
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      - in: query
        name: ReplicationTaskIdentifier
        description: The replication task identifier
        type: string
      - in: query
        name: ReplicationTaskSettings
        description: Settings for the task, such as target metadata settings
        type: string
      - in: query
        name: SourceEndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: TableMappings
        description: The path of the JSON file that contains the table mappings
        type: string
      - in: query
        name: Tags
        description: Tags to be added to the replication instance
        type: string
      - in: query
        name: TargetEndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=DeleteReplicationTask:
    get:
      summary: Delete Replication Task
      description: Deletes the specified replication task.
      operationId: deleteReplicationTask
      x-api-path-slug: actiondeletereplicationtask-get
      parameters:
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task to be
          deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=DescribeReplicationTasks:
    get:
      summary: Describe Replication Tasks
      description: Returns information about replication tasks for your account in
        the current region.
      operationId: describeReplicationTasks
      x-api-path-slug: actiondescribereplicationtasks-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous     request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=ModifyReplicationTask:
    get:
      summary: Modify Replication Task
      description: Modifies the specified replication task.
      operationId: modifyReplicationTask
      x-api-path-slug: actionmodifyreplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: MigrationType
        description: The migration type
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task
        type: string
      - in: query
        name: ReplicationTaskIdentifier
        description: The replication task identifier
        type: string
      - in: query
        name: ReplicationTaskSettings
        description: JSON file that contains settings for the task, such as target
          metadata settings
        type: string
      - in: query
        name: TableMappings
        description: The path of the JSON file that contains the table mappings
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=StartReplicationTask:
    get:
      summary: Start Replication Task
      description: Starts the replication task.
      operationId: startReplicationTask
      x-api-path-slug: actionstartreplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number (ARN) of the replication task to be
          started
        type: string
      - in: query
        name: StartReplicationTaskType
        description: The type of replication task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=StopReplicationTask:
    get:
      summary: Stop Replication Task
      description: Stops the replication task.
      operationId: stopReplicationTask
      x-api-path-slug: actionstopreplicationtask-get
      parameters:
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number(ARN) of the replication task to be
          stopped
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
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