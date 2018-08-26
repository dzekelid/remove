---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Remove Rejected Sender
  description: Remove rejectedSender Remove a user or group from the rejectedSenders
    list.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{id}/acceptedSenders/$ref:
    delete:
      summary: Remove Accepted Sender
      description: Remove acceptedSender Remove a user or group from the acceptedSenders
        list.
      operationId: RemoveAcceptedSender
      x-api-path-slug: groupsidacceptedsendersref-delete
      parameters:
      - in: query
        name: $id
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: gt;
        type: string
      - in: path
        name: id
        type: string
      - in: query
        name: lt;id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Accepted
      - Sender
  /groups/{id}/members/{id}/$ref:
    delete:
      summary: Remove Member
      description: Remove member Use this API to remove a member from an Office 365
        group, a security group or a mail-enabled security group through the members
        navigation property. You can remove users or other groups.
      operationId: RemoveMember
      x-api-path-slug: groupsidmembersidref-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Member
  /groups/{id}/owners/{id}/$ref:
    delete:
      summary: Remove Owner
      description: Remove owner Use this API to remove an owner from an Office 365
        group, a security group or a mail-enabled security group through the owners
        navigation property.
      operationId: RemoveOwner
      x-api-path-slug: groupsidownersidref-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Owner
  /groups/{id}/rejectedSenders/$ref:
    delete:
      summary: Remove Rejected Sender
      description: Remove rejectedSender Remove a user or group from the rejectedSenders
        list.
      operationId: RemoveRejectedSender
      x-api-path-slug: groupsidrejectedsendersref-delete
      parameters:
      - in: query
        name: $id
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: gt;
        type: string
      - in: path
        name: id
        type: string
      - in: query
        name: lt;id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Rejected
      - Sender
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