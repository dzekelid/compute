---
name: AWS Directory Service
description: AWS Directory Service for Microsoft Active Directory (Enterprise Edition),
  also known as AWS Microsoft AD, enables your directory-aware workloads and AWS resources
  to use managed Active Directory in the AWS Cloud. The Microsoft AD service is built
  on actual Microsoft Active Directory and does not require you to synchronize or
  replicate data from your existing Active Directory to the cloud. You can use standard
  Active Directory administration tools and take advantage of built-in Active Directory
  features such as Group Policy, trusts, and single sign-on. With Microsoft AD, you
  can easily joinnbsp;Amazon EC2nbsp;andnbsp;Amazon RDS for SQL Servernbsp;instances
  to a domain, and usenbsp;AWS Enterprise IT applicationsnbsp;such asnbsp;Amazon WorkSpacesnbsp;with
  Active Directory users and groups.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Security
- Discovery
- Authentication
- Amazon Web Services
created: "2018-03-13"
modified: "2018-03-13"
url: https://raw.githubusercontent.com/streamdata-gallery/compute/master/_listings/aws-directory-service/apis.yaml
specificationVersion: "0.14"
apis:
- name: AWS Directory Service API
  description: AWS Directory Service for Microsoft Active Directory (Enterprise Edition),
    also known as AWS Microsoft AD, enables your directory-aware workloads and AWS
    resources to use managed Active Directory in the AWS Cloud
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
  humanURL: ""
  baseURL: :///
  tags: Compute
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/compute/master/_listings/aws-directory-service/action-createcomputer-get.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/ds/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/directoryservice/latest/devguide/api-ref.html
- type: x-faq
  url: https://aws.amazon.com/directoryservice/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/directoryservice/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/directoryservice/pricing/
- type: x-website
  url: https://aws.amazon.com/directoryservice/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---