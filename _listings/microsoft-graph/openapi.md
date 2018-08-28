swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
  /groups/{id}/removeFavorite:
    post:
      summary: Group Remove Favorite
      description: 'group: removeFavorite Remove the group from the list of the current
        user''s favorite groups. Supported for only Office 365 groups.'
      operationId: Group:RemoveFavorite
      x-api-path-slug: groupsidremovefavorite-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Remove
      - Favorite