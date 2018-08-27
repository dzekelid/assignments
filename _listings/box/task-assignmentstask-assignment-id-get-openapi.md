---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Task Assignment
  description: Fetches a specific task assignment.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tasks/{TASK_ID}/assignments:
    get:
      summary: Get Assignments
      description: Retrieves all of the assignments for a given task.
      operationId: getTaskAssignments
      x-api-path-slug: taskstask-idassignments-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: TASK_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Tasks
      - Task
      - ""
      - Assignments
  /task_assignments:
    post:
      summary: Create Task Assignment
      description: Used to assign a task to a single user. There can be multiple assignments
        on a given task.
      operationId: createTaskAssignment
      x-api-path-slug: task-assignments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Task
      - Assignments
  /task_assignments/{TASK_ASSIGNMENT_ID}:
    get:
      summary: Get Task Assignment
      description: Fetches a specific task assignment.
      operationId: getTaskAssignment
      x-api-path-slug: task-assignmentstask-assignment-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: TASK_ASSIGNMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Task
      - Assignments
      - Task
      - Assignment
    put:
      summary: Update Task Assignment
      description: Used to update a task assignment.
      operationId: updateTaskAssignment
      x-api-path-slug: task-assignmentstask-assignment-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: TASK_ASSIGNMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Task
      - Assignments
      - Task
      - Assignment
    delete:
      summary: Delete Task Assignment
      description: Deletes a specific task assignment.
      operationId: deleteTaskAssignment
      x-api-path-slug: task-assignmentstask-assignment-id-delete
      parameters:
      - in: path
        name: TASK_ASSIGNMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Task
      - Assignments
      - Task
      - Assignment
  /retention_policies/{POLICY_ID}/assignments:
    get:
      summary: Get Retention Policy Assignments
      description: Returns a list of all retention policy assignments associated with
        a specified retention policy.
      operationId: getRetentionPolicyAssignments
      x-api-path-slug: retention-policiespolicy-idassignments-get
      parameters:
      - in: path
        name: POLICY_ID
      - in: query
        name: type
        description: The type of the retention policy assignment to retrieve
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Retention
      - Policies
      - Policy
      - ""
      - Assignments
  /retention_policy_assignments:
    post:
      summary: Create Retention Policy Assignment
      description: Returns a list of all retention policy assignments associated with
        a specified retention policy.
      operationId: createRetentionPolicyAssignment
      x-api-path-slug: retention-policy-assignments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Retention
      - Policy
      - Assignments
  /retention_policy_assignments/{RETENTION_POLICY_ASSIGNMENT_ID}:
    get:
      summary: Get Retention Policy Assignment
      description: Used to retrieve information about a retention policy assignment.
      operationId: getRetentionPolicyAssignment
      x-api-path-slug: retention-policy-assignmentsretention-policy-assignment-id-get
      parameters:
      - in: path
        name: RETENTION_POLICY_ASSIGNMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Retention
      - Policy
      - Assignments
      - Retention
      - Policy
      - Assignment
  /legal_hold_policies/{ID}/assignments:
    get:
      summary: Get Legal hold policy assignments
      description: Get list of assignments for a single Policy.
      operationId: getLegalHoldPolicyAssignments
      x-api-path-slug: legal-hold-policiesidassignments-get
      parameters:
      - in: path
        name: ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Legal
      - Hold
      - Policies
      - ""
      - Assignments
  /legal_hold_policy_assignments:
    post:
      summary: Create New Legal Hold Policy Assignment
      description: Create a new Assignment, which will apply the Legal Hold Policy
        to the target of the Assignment.
      operationId: createLegalHoldPolicyAssignment
      x-api-path-slug: legal-hold-policy-assignments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Legal
      - Hold
      - Policy
      - Assignments
  /legal_hold_policy_assignments/{ASSIGNMENT_ID}:
    get:
      summary: Get Legal Hold Policy Assignment
      description: Get details of a single assignment.
      operationId: getLegalHoldPolicyAssignment
      x-api-path-slug: legal-hold-policy-assignmentsassignment-id-get
      parameters:
      - in: path
        name: ASSIGNMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Legal
      - Hold
      - Policy
      - Assignments
      - Assignment
    delete:
      summary: Delete Legal Hold Policy Assignment
      description: Sends request to delete an existing Assignment. Note that this
        is an asynchronous process - the Assignment will not be fully deleted yet
        when the response comes back.
      operationId: deleteLegalHoldPolicyAssignment
      x-api-path-slug: legal-hold-policy-assignmentsassignment-id-delete
      parameters:
      - in: path
        name: ASSIGNMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Legal
      - Hold
      - Policy
      - Assignments
      - Assignment
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---