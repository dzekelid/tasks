---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---