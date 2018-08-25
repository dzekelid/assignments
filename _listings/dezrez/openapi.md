---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/assignleadsforspecifiednegs:
    put:
      summary: Assign InboundLead Todos to all the specified Negs using round-robin
        assignement.
      description: Assign inboundlead todos to all the specified negs using round-robin
        assignement..
      operationId: DefaultToDo_AssignLeadsForSpecifiedNegsByassignPropertyLeadsCommandDataContract
      x-api-path-slug: apitodoassignleadsforspecifiednegs-put
      parameters:
      - in: body
        name: assignPropertyLeadsCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Assign
      - InboundLead
      - Todos
      - To
      - ""
      - Specified
      - Negs
      - Using
      - Round-robin
      - Assignement
  /api/inboundlead/create:
    post:
      summary: Creates a lead in the system, optinally assigning the lead to a negotiator
      description: Creates a lead in the system, optinally assigning the lead to a
        negotiator.
      operationId: InboundLead_CreateLeadBydataContractByassignToNegId
      x-api-path-slug: apiinboundleadcreate-post
      parameters:
      - in: query
        name: assignToNegId
        description: Negotiator Id to assign lead too
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Lead
      - In
      - System
      - ""
      - Optinally
      - Assigning
      - Lead
      - To
      - Negotiator
---