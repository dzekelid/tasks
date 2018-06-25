---
name: AWS Data Pipeline
x-slug: aws-data-pipeline
description: AWS Data Pipeline is a web service that helps you reliably process and
  move data between different AWS compute and storage services, as well as on-premise
  data sources, at specified intervals. With AWS Data Pipeline, you can regularly
  access your data where it&rsquo;s stored, transform and process it at scale, and
  efficiently transfer the results to AWS services such as Amazon S3, Amazon RDS,
  Amazon DynamoDB, and Amazon EMR.AWS Data Pipeline helps you easily create complex
  data processing workloads that are fault tolerant, repeatable, and highly available.
  You don&rsquo;t have to worry about ensuring resource availability, managing inter-task
  dependencies, retrying transient failures or timeouts in individual tasks, or creating
  a failure notification system. AWS Data Pipeline also allows you to move and process
  data that was previously locked up in on-premise data silos.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tasks
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-data-pipeline/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Data Pipeline API Poll For Task
  x-api-slug: aws-data-pipeline-api
  description: Task runners call PollForTask to receive a task to perform from AWS
    Data Pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=PollForTask
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-data-pipeline/actionpollfortask-get-openapi.md
- name: AWS Data Pipeline API Report Task Progress
  x-api-slug: aws-data-pipeline-api
  description: Task runners call ReportTaskProgress when assigned a task to acknowledge
    that it has the task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=ReportTaskProgress
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-data-pipeline/actionreporttaskprogress-get-openapi.md
- name: AWS Data Pipeline API Set Task Status
  x-api-slug: aws-data-pipeline-api
  description: Task runners call SetTaskStatus to notify AWS Data Pipeline that a
    task is completed and provide information about the final status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: ://///?Action=SetTaskStatus
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-data-pipeline/actionsettaskstatus-get-openapi.md
- name: AWS Data Pipeline API
  x-api-slug: aws-data-pipeline-api
  description: AWS Data Pipeline is a web service that helps you reliably process
    and move data between different AWS compute and storage services, as well as on-premise
    data sources, at specified intervals. With AWS Data Pipeline, you can regularly
    access your data where it&rsquo;s stored, transform and process it at scale, and
    efficiently transfer the results to AWS services such as Amazon S3, Amazon RDS,
    Amazon DynamoDB, and Amazon EMR.AWS Data Pipeline helps you easily create complex
    data processing workloads that are fault tolerant, repeatable, and highly available.
    You don&rsquo;t have to worry about ensuring resource availability, managing inter-task
    dependencies, retrying transient failures or timeouts in individual tasks, or
    creating a failure notification system. AWS Data Pipeline also allows you to move
    and process data that was previously locked up in on-premise data silos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-data-pipeline/openapi.md
x-common:
- type: x-blog
  url: http://blogs.aws.amazon.com/bigdata
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/AWS-Data-Pipeline/
- type: x-documentation
  url: http://docs.aws.amazon.com/datapipeline/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/datapipeline/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=151
- type: x-pricing
  url: https://aws.amazon.com/datapipeline/pricing/
- type: x-tools
  url: http://aws.amazon.com/developertools/AWS-Data-Pipeline/
- type: x-website
  url: https://aws.amazon.com/datapipeline/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---