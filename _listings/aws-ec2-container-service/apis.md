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
x-alexaRank: ""
tags: State
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-container-service/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon EC2 Container Service API Submit Container State Change
  x-api-slug: amazon-ec2-container-service-api
  description: This action is only used by the Amazon EC2 Container Service agent,
    and it is not intended for use outside of the agent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=SubmitContainerStateChange
  tags: Container State Change
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-container-service/actionsubmitcontainerstatechange-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-container-service/actionsubmitcontainerstatechange-get-openapi.md
- name: Amazon EC2 Container Service API Submit Task State Change
  x-api-slug: amazon-ec2-container-service-api
  description: This action is only used by the Amazon EC2 Container Service agent,
    and it is not intended for use outside of the agent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECS.png
  humanURL: https://aws.amazon.com/ecs/
  baseURL: ://///?Action=SubmitTaskStateChange
  tags: Task State Change
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-container-service/actionsubmittaskstatechange-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-container-service/actionsubmittaskstatechange-get-openapi.md
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
  tags: State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-container-service/openapi.md
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