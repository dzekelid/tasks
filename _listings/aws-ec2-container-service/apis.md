---
name: AWS EC2 Container Service
x-slug: aws-ec2-container-service
description: Amazon EC2 Container Service (ECS) is a highly scalable, high performance
  container management service that supports Docker containers and allows you to easily
  run applications on a managed cluster of Amazon EC2 instances. Amazon ECS eliminates
  the need for you to install, operate, and scale your own cluster management infrastructure.
  With simple API calls, you can launch and stop Docker-enabled applications, query
  the complete state of your cluster, and access many familiar features like security
  groups, Elastic Load Balancing, EBS volumes, and IAM roles. You can use Amazon ECS
  to schedule the placement of containers across your cluster based on your resource
  needs and availability requirements. You can also integrate your own scheduler or
  third-party schedulers to meet business or application specific requirements.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tasks
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon EC2 Container Service API Describe Tasks
  x-api-slug: amazon-ec2-container-service-api
  description: Describes a specified task or tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=DescribeTasks
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/actiondescribetasks-get-openapi.md
- name: Amazon EC2 Container Service API List Tasks
  x-api-slug: amazon-ec2-container-service-api
  description: Returns a list of tasks for a specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=ListTasks
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/actionlisttasks-get-openapi.md
- name: Amazon EC2 Container Service API Run Task
  x-api-slug: amazon-ec2-container-service-api
  description: Starts a new task using the specified task definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=RunTask
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/actionruntask-get-openapi.md
- name: Amazon EC2 Container Service API Start Task
  x-api-slug: amazon-ec2-container-service-api
  description: |-
    Starts a new task from the specified task definition on the specified container
                instance or instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=StartTask
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/actionstarttask-get-openapi.md
- name: Amazon EC2 Container Service API Stop Task
  x-api-slug: amazon-ec2-container-service-api
  description: Stops a running task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=StopTask
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/actionstoptask-get-openapi.md
- name: Amazon EC2 Container Service API
  x-api-slug: amazon-ec2-container-service-api
  description: Amazon EC2 Container Service (ECS) is a highly scalable, high performance
    container management service that supports Docker containers and allows you to
    easily run applications on a managed cluster of Amazon EC2 instances. Amazon ECS
    eliminates the need for you to install, operate, and scale your own cluster management
    infrastructure. With simple API calls, you can launch and stop Docker-enabled
    applications, query the complete state of your cluster, and access many familiar
    features like security groups, Elastic Load Balancing, EBS volumes, and IAM roles.
    You can use Amazon ECS to schedule the placement of containers across your cluster
    based on your resource needs and availability requirements. You can also integrate
    your own scheduler or third-party schedulers to meet business or application specific
    requirements.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: :///
  tags: Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tasks/master/_listings/aws-ec2-container-service/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonECS/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/ecs/faqs/
- type: x-getting-started
  url: https://portal.aws.amazon.com/gp/aws/developer/registration/index.html
- type: x-pricing
  url: https://aws.amazon.com/ecs/pricing/
- type: x-website
  url: https://aws.amazon.com/ecs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---