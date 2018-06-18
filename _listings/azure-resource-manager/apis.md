---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Assignments
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API Policy Assignments Delete
  x-api-slug: azure-resource-manager-api
  description: Deletes a policy assignment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-delete-openapi.md
- name: Azure Resource Manager API Creates a policy assignment.
  x-api-slug: azure-resource-manager-api
  description: Policy assignments are inherited by child resources. For example, when
    you apply a policy to a resource group that policy is assigned to all resources
    in the group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}
  tags: Policy Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-put-openapi.md
- name: Azure Resource Manager API Policy Assignments Get
  x-api-slug: azure-resource-manager-api
  description: Gets a policy assignment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{scope}/providers/Microsoft.Authorization/policyassignments/{policyAssignmentName}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-authorizationpolicyassignmentspolicyassignmentname-get-openapi.md
- name: Azure Resource Manager API Policy Assignments List For Resource Group
  x-api-slug: azure-resource-manager-api
  description: Gets policy assignments for the resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Authorization/policyAssignments
  tags: Policy Assignments For Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationpolicyassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-authorizationpolicyassignments-get-openapi.md
- name: Azure Resource Manager API Policy Assignments List For Resource
  x-api-slug: azure-resource-manager-api
  description: Gets policy assignments for a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}/providers/Microsoft.Authorization/policyassignments
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationpolicyassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcenameprovidersmicrosoft-authorizationpolicyassignments-get-openapi.md
- name: Azure Resource Manager API Policy Assignments List
  x-api-slug: azure-resource-manager-api
  description: Gets all the policy assignments for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Authorization/policyassignments
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicyassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-authorizationpolicyassignments-get-openapi.md
- name: Azure Resource Manager API Deletes a policy assignment by ID.
  x-api-slug: azure-resource-manager-api
  description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{policyAssignmentId}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-delete-openapi.md
- name: Azure Resource Manager API Creates a policy assignment by ID.
  x-api-slug: azure-resource-manager-api
  description: Policy assignments are inherited by child resources. For example, when
    you apply a policy to a resource group that policy is assigned to all resources
    in the group. When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{policyAssignmentId}
  tags: Policy Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-put-openapi.md
- name: Azure Resource Manager API Gets a policy assignment by ID.
  x-api-slug: azure-resource-manager-api
  description: When providing a scope for the assigment, use '/subscriptions/{subscription-id}/'
    for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}'
    for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}'
    for resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////{policyAssignmentId}
  tags: Policy Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/policyassignmentid-get-openapi.md
- name: Azure Resource Manager API
  x-api-slug: azure-resource-manager-api
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions. You organize related resources in resource groups, and
    deploy your resources with JSON templates. For an introduction to deploying and
    managing resources with Resource Manager, see Azure Resource Manager overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/azure-resource-manager/openapi.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---