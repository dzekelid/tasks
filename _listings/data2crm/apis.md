---
name: Data2CRM
x-slug: data2crm
description: Data2CRM is all-in-one master touch instrument to create the perfect
  data environment for prosperous internal and external connections.Data2CRM.API,
  a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tasks
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/apis.md
specificationVersion: "0.14"
apis:
- name: Data2CRM GET for Task
  x-api-slug: data2crm
  description: Returns all tasks from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task
  tags: Tasks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/task-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/task-get-openapi.md
- name: Data2CRM POST for Task
  x-api-slug: data2crm
  description: Add task into the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/task-post-openapi.md
- name: Data2CRM COUNT for Task
  x-api-slug: data2crm
  description: Count all tasks from the system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task/count
  tags: Tasks,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/taskcount-get-openapi.md
- name: Data2CRM DESCRIBE for Task
  x-api-slug: data2crm
  description: Returns describe for tasks
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task/describe
  tags: Tasks,Describe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/taskdescribe-get-openapi.md
- name: Data2CRM DELETE for Task
  x-api-slug: data2crm
  description: Delete task information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task/{task_id}
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/tasktask-id-delete-openapi.md
- name: Data2CRM GET for Task
  x-api-slug: data2crm
  description: Return task information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task/{task_id}
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/tasktask-id-get-openapi.md
- name: Data2CRM PUT for Task
  x-api-slug: data2crm
  description: Update task information
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1//task/{task_id}
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/tasktask-id-put-openapi.md
- name: Data2CRM
  x-api-slug: data2crm
  description: Data2CRM is all-in-one master touch instrument to create the perfect
    data environment for prosperous internal and external connections.Data2CRM.API,
    a Unified API Provider, to Connect Your Business Software with 17+ CRMs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data2crm-logo.png
  humanURL: http://data2crm.com
  baseURL: https://api.data2crm.com:80//v1
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/data2crm/openapi.md
x-common:
- type: x-twitter
  url: https://twitter.com/data2crm
- type: x-website
  url: http://data2crm.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---