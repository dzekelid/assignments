---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Delete Task Assignment
  description: Deletes a specific task assignment.
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