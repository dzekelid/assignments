swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/assignee:
    put:
      summary: Assign issue
      description: Assigns the issue to the user. Use this resource to assign issues
        for the users having "Assign Issue" permission, and not having the "Edit Issue"
        permission. If `name` body parameter is set to "-1" then automatic issue assignee
        is used. A `name` set to `null` will remove the assignee.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.assignIssue_put
      x-api-path-slug: api2issueissueidorkeyassignee-put
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be updated
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Issue