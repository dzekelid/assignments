---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "445"
tags: Assignments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box Get Assignments
  x-api-slug: box
  description: Retrieves all of the assignments for a given task.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//tasks/{TASK_ID}/assignments
  tags: Documents,Tasks, Task, , Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/taskstask-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/taskstask-idassignments-get-openapi.md
- name: Box Create Task Assignment
  x-api-slug: box
  description: Used to assign a task to a single user. There can be multiple assignments
    on a given task.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//task_assignments
  tags: Documents,Task, Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/task-assignments-post-openapi.md
- name: Box Get Task Assignment
  x-api-slug: box
  description: Fetches a specific task assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//task_assignments/{TASK_ASSIGNMENT_ID}
  tags: Documents,Task, Assignments, Task, Assignment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/task-assignmentstask-assignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/task-assignmentstask-assignment-id-get-openapi.md
- name: Box Update Task Assignment
  x-api-slug: box
  description: Used to update a task assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//task_assignments/{TASK_ASSIGNMENT_ID}
  tags: Documents,Task, Assignments, Task, Assignment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/task-assignmentstask-assignment-id-put-openapi.md
- name: Box Delete Task Assignment
  x-api-slug: box
  description: Deletes a specific task assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//task_assignments/{TASK_ASSIGNMENT_ID}
  tags: Documents,Task, Assignments, Task, Assignment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/task-assignmentstask-assignment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/task-assignmentstask-assignment-id-delete-openapi.md
- name: Box Get Retention Policy Assignments
  x-api-slug: box
  description: Returns a list of all retention policy assignments associated with
    a specified retention policy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//retention_policies/{POLICY_ID}/assignments
  tags: Documents,Retention, Policies, Policy, , Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/retention-policiespolicy-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/retention-policiespolicy-idassignments-get-openapi.md
- name: Box Create Retention Policy Assignment
  x-api-slug: box
  description: Returns a list of all retention policy assignments associated with
    a specified retention policy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//retention_policy_assignments
  tags: Documents,Retention, Policy, Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/retention-policy-assignments-post-openapi.md
- name: Box Get Retention Policy Assignment
  x-api-slug: box
  description: Used to retrieve information about a retention policy assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//retention_policy_assignments/{RETENTION_POLICY_ASSIGNMENT_ID}
  tags: Documents,Retention, Policy, Assignments, Retention, Policy, Assignment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/retention-policy-assignmentsretention-policy-assignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/retention-policy-assignmentsretention-policy-assignment-id-get-openapi.md
- name: Box Get Legal hold policy assignments
  x-api-slug: box
  description: Get list of assignments for a single Policy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//legal_hold_policies/{ID}/assignments
  tags: Documents,Legal, Hold, Policies, , Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policiesidassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policiesidassignments-get-openapi.md
- name: Box Create New Legal Hold Policy Assignment
  x-api-slug: box
  description: Create a new Assignment, which will apply the Legal Hold Policy to
    the target of the Assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//legal_hold_policy_assignments
  tags: Documents,Legal, Hold, Policy, Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policy-assignments-post-openapi.md
- name: Box Get Legal Hold Policy Assignment
  x-api-slug: box
  description: Get details of a single assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//legal_hold_policy_assignments/{ASSIGNMENT_ID}
  tags: Documents,Legal, Hold, Policy, Assignments, Assignment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policy-assignmentsassignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policy-assignmentsassignment-id-get-openapi.md
- name: Box Delete Legal Hold Policy Assignment
  x-api-slug: box
  description: Sends request to delete an existing Assignment. Note that this is an
    asynchronous process - the Assignment will not be fully deleted yet when the response
    comes back.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//legal_hold_policy_assignments/{ASSIGNMENT_ID}
  tags: Documents,Legal, Hold, Policy, Assignments, Assignment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policy-assignmentsassignment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/legal-hold-policy-assignmentsassignment-id-delete-openapi.md
- name: Box
  x-api-slug: box
  description: Box.net provides a sophisticated API for their online document sharing
    and collaboration web application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/box/openapi.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---