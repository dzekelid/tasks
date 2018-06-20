---
name: AWS Database Migration Service
x-slug: aws-database-migration-service
description: AWS Database Migration Service helps you migrate databases to AWS easily
  and securely. The source database remains fully operational during the migration,
  minimizing downtime to applications that rely on the database. The AWS Database
  Migration Service can migrate your data to and from most widely used commercial
  and open-source databases. The service supports homogenous migrations such as Oracle
  to Oracle, as well as heterogeneous migrations between different database platforms,
  such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It also allows
  you to stream data to Amazon Redshift from any of the supported sources including
  Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE and SQL Server, enabling
  consolidation and easy analysis of data in the petabyte-scale data warehouse. AWS
  Database Migration Service can also be used for continuous data replication with
  high-availability.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tasks
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Database Migration Service API Create Replication Task
  x-api-slug: aws-database-migration-service-api
  description: Creates a replication task using the specified parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=CreateReplicationTask
  tags: Replication Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/actioncreatereplicationtask-get-openapi.md
- name: AWS Database Migration Service API Delete Replication Task
  x-api-slug: aws-database-migration-service-api
  description: Deletes the specified replication task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=DeleteReplicationTask
  tags: Replication Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/actiondeletereplicationtask-get-openapi.md
- name: AWS Database Migration Service API Describe Replication Tasks
  x-api-slug: aws-database-migration-service-api
  description: Returns information about replication tasks for your account in the
    current region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=DescribeReplicationTasks
  tags: Replication Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/actiondescribereplicationtasks-get-openapi.md
- name: AWS Database Migration Service API Modify Replication Task
  x-api-slug: aws-database-migration-service-api
  description: Modifies the specified replication task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=ModifyReplicationTask
  tags: Replication Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/actionmodifyreplicationtask-get-openapi.md
- name: AWS Database Migration Service API Start Replication Task
  x-api-slug: aws-database-migration-service-api
  description: Starts the replication task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=StartReplicationTask
  tags: Replication Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/actionstartreplicationtask-get-openapi.md
- name: AWS Database Migration Service API Stop Replication Task
  x-api-slug: aws-database-migration-service-api
  description: Stops the replication task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=StopReplicationTask
  tags: Replication Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/actionstopreplicationtask-get-openapi.md
- name: AWS Database Migration Service API
  x-api-slug: aws-database-migration-service-api
  description: AWS Database Migration Service helps you migrate databases to AWS easily
    and securely. The source database remains fully operational during the migration,
    minimizing downtime to applications that rely on the database. The AWS Database
    Migration Service can migrate your data to and from most widely used commercial
    and open-source databases. The service supports homogenous migrations such as
    Oracle to Oracle, as well as heterogeneous migrations between different database
    platforms, such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It
    also allows you to stream data to Amazon Redshift from any of the supported sources
    including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE and SQL Server,
    enabling consolidation and easy analysis of data in the petabyte-scale data warehouse.
    AWS Database Migration Service can also be used for continuous data replication
    with high-availability.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: :///
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-database-migration-service/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/dms/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/dms/getting-started/
- type: x-partners
  url: https://aws.amazon.com/dms/partners/
- type: x-pricing
  url: https://aws.amazon.com/dms/pricing/
- type: x-schema-conversion
  url: https://aws.amazon.com/dms/#sct
- type: x-testimonials
  url: https://aws.amazon.com/dms/testimonials/
- type: x-website
  url: https://aws.amazon.com/dms/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---