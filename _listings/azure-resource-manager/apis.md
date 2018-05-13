---
name: Azure Resource Manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Resources
- Microsoft
- Links
- Deployment
created: "2018-03-27"
modified: "2018-03-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/apis.yaml
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-get.md
- name: Azure Resource Manager API
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/scope-providers-microsoft-authorization-policyassignments-policyassignmentname-put.md
- name: Azure Resource Manager API Gets a policy assignment by ID.
  description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: http:://management.azure.com//
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-get-postman.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---