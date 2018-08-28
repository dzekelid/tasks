---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Describe Import Image Tasks
  version: 1.0.0
  description: Displays details about an import virtual machine or import snapshot
    tasks that are already created.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeBundleTasks:
    get:
      summary: Describe Bundle Tasks
      description: Describes one or more of your bundling tasks.
      operationId: describebundletasks
      x-api-path-slug: actiondescribebundletasks-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of an EC2-Classic instance to link to the ClassicLink-enabled
          VPC
        type: string
      - in: query
        name: SecurityGroupId.N
        description: The ID of one or more of the VPCs security groups
        type: string
      - in: query
        name: VpcId
        description: The ID of a ClassicLink-enabled VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Task
  /?Action=DescribeConversionTasks:
    get:
      summary: Describe Conversion Tasks
      description: Describes one or more of your conversion tasks.
      operationId: describeconversiontasks
      x-api-path-slug: actiondescribeconversiontasks-get
      responses:
        200:
          description: OK
      tags:
      - Version Tasks
  /?Action=DescribeExportTasks:
    get:
      summary: Describe Export Tasks
      description: Describes one or more of your export tasks.
      operationId: describeexporttasks
      x-api-path-slug: actiondescribeexporttasks-get
      parameters:
      - in: query
        name: AmazonProvidedIpv6CidrBlock
        description: Requests an Amazon-provided IPv6 CIDR block with a /56 prefix
          length for the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Takss
  /?Action=DescribeImportImageTasks:
    get:
      summary: Describe Import Image Tasks
      description: Displays details about an import virtual machine or import snapshot
        tasks that are already created.
      operationId: describeimportimagetasks
      x-api-path-slug: actiondescribeimportimagetasks-get
      responses:
        200:
          description: OK
      tags:
      - Import Image Tasks
  /?Action=DescribeImportSnapshotTasks:
    get:
      summary: Describe Import Snapshot Tasks
      description: Describes your import snapshot tasks.
      operationId: describeimportsnapshottasks
      x-api-path-slug: actiondescribeimportsnapshottasks-get
      parameters:
      - in: query
        name: Description
        description: A description for the instance being imported
        type: string
      - in: query
        name: DiskImage.N
        description: The disk image
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      - in: query
        name: LaunchSpecification
        description: The launch specification
        type: string
      - in: query
        name: Platform
        description: The instance operating system
        type: string
      responses:
        200:
          description: OK
      tags:
      - Import Snapshot Takss
  /?Action=CancelBundleTask:
    get:
      summary: Cancel Bundle Task
      description: Cancels a bundling operation for an instance store-backed Windows
        instance.
      operationId: cancelbundletask
      x-api-path-slug: actioncancelbundletask-get
      parameters:
      - in: query
        name: BundleId.N
        description: One or more bundle task IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Task
  /?Action=CancelConversionTask:
    get:
      summary: Cancel Conversion Task
      description: Cancels an active conversion task.
      operationId: cancelconversiontask
      x-api-path-slug: actioncancelconversiontask-get
      responses:
        200:
          description: OK
      tags:
      - Bundle Task
  /?Action=CancelExportTask:
    get:
      summary: Cancel Export Task
      description: Cancels an active export task.
      operationId: cancelexporttask
      x-api-path-slug: actioncancelexporttask-get
      parameters:
      - in: query
        name: Description
        description: A description for the conversion task or the resource being exported
        type: string
      - in: query
        name: ExportToS3
        description: The format and location for an instance export task
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: TargetEnvironment
        description: The target virtualization environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Task
  /?Action=CancelImportTask:
    get:
      summary: Cancel Import Task
      description: Cancels an in-process import virtual machine or import snapshot
        task.
      operationId: cancelimporttask
      x-api-path-slug: actioncancelimporttask-get
      parameters:
      - in: query
        name: ConversionTaskId.N
        description: One or more conversion task IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Import Task
  /?Action=CreateInstanceExportTask:
    get:
      summary: Create Instance Export Task
      description: Exports a running or stopped instance to an S3 bucket.
      operationId: createinstanceexporttask
      x-api-path-slug: actioncreateinstanceexporttask-get
      parameters:
      - in: query
        name: ExportTaskId.N
        description: One or more export task IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Task
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