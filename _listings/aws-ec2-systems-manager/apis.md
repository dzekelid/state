---
name: AWS EC2 Systems Manager
x-slug: aws-ec2-systems-manager
description: Amazon EC2 Systems Manager is a management service that helps you automatically
  collect software inventory, apply OS patches, create system images, and configure
  Windows and Linux operating systems. These capabilities help you define and track
  system configurations, prevent drift, and maintain software compliance of your EC2
  and on-premises configurations. By providing a management approach that is designed
  for the scale and agility of the cloud but extends into your on-premises data center,
  EC2 Systems Manager makes it easier for you to seamlessly bridge your existing infrastructure
  with AWS.EC2 Systems Manager is easy to use. Simply access EC2 Systems Manager from
  the EC2 Management Console, select the instances you want to manage, and define
  the management tasks you want to perform. EC2 Systems Manager is available now at
  no cost to manage both your EC2 and on-premises resources.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
x-kinRank: "10"
x-alexaRank: ""
tags: State
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-systems-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon EC2 Systems Manager API Describe Instance Patch States
  x-api-slug: amazon-ec2-systems-manager-api
  description: Retrieves the high-level patch state of one or more instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DescribeInstancePatchStates
  tags: Instance, States
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-systems-manager/actiondescribeinstancepatchstates-get-openapi.md
- name: Amazon EC2 Systems Manager API Describe Instance Patch States For Patch Group
  x-api-slug: amazon-ec2-systems-manager-api
  description: Retrieves the high-level patch state for the instances in the specified
    patch group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DescribeInstancePatchStatesForPatchGroup
  tags: Instance, StatesGroup
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-systems-manager/actiondescribeinstancepatchstatesforpatchgroup-get-openapi.md
- name: Amazon EC2 Systems Manager API Describe Patch Group State
  x-api-slug: amazon-ec2-systems-manager-api
  description: Returns high-level aggregated patch compliance state for a patch group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: ://///?Action=DescribePatchGroupState
  tags: Group, State
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-systems-manager/actiondescribepatchgroupstate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-systems-manager/actiondescribepatchgroupstate-get-openapi.md
- name: Amazon EC2 Systems Manager API
  x-api-slug: amazon-ec2-systems-manager-api
  description: Amazon EC2 Systems Manager is a management service that helps you automatically
    collect software inventory, apply OS patches, create system images, and configure
    Windows and Linux operating systems. These capabilities help you define and track
    system configurations, prevent drift, and maintain software compliance of your
    EC2 and on-premises configurations. By providing a management approach that is
    designed for the scale and agility of the cloud but extends into your on-premises
    data center, EC2 Systems Manager makes it easier for you to seamlessly bridge
    your existing infrastructure with AWS.EC2 Systems Manager is easy to use. Simply
    access EC2 Systems Manager from the EC2 Management Console, select the instances
    you want to manage, and define the management tasks you want to perform. EC2 Systems
    Manager is available now at no cost to manage both your EC2 and on-premises resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/systems-manager/
  baseURL: :///
  tags: State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/aws-ec2-systems-manager/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/ssm/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/ec2/systems-manager/faqs/
- type: x-getting-started
  url: http://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/systems-manager.html
- type: x-website
  url: https://aws.amazon.com/ec2/systems-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---