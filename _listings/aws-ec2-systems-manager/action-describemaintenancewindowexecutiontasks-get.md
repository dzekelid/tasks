---
swagger: "2.0"
info:
  title: Amazon EC2 Systems Manager API Describe Maintenance Window Execution Tasks
  version: 1.0.0
  description: For a given Maintenance Window execution, lists the tasks that were
    executed.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeMaintenanceWindowExecutionTasks:
    get:
      summary: ' Describe Maintenance Window Execution Tasks '
      description: For a given Maintenance Window execution, lists the tasks that
        were executed
      operationId: describeMaintenanceWindowExecutionTasks
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
      - maintenance
      - window
      - execution
      - tasks
definitions: []
x-collection-name: AWS EC2 Systems Manager
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