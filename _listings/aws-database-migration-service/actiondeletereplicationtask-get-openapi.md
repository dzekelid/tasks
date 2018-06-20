---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 0
info:
  title: AWS Database Migration Service API Delete Replication Task
  version: 1.0.0
  description: Deletes the specified replication task.
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