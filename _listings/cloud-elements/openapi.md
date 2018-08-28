swagger: "2.0"
x-collection-name: Cloud Elements
x-complete: 1
info:
  title: zohocrm
  version: api-v2
host: console.cloud-elements.com
basePath: /elements/api-v2/hubs/crm
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/remove:
    post:
      summary: Remove
      description: Remove.
      operationId: postMembersRemove
      x-api-path-slug: membersremove-post
      parameters:
      - in: query
        name: delete_data
        description: optional controls if the users data will be deleted on their
          linked devices
      - in: query
        name: external_id
        description: optional external ID
      - in: query
        name: member_id
        description: optional member ID
      - in: query
        name: transfer_admin_member_id
        description: optional errors during the transfer process will be sent via
          email to the transfer_admin_member_id
      - in: query
        name: transfer_dest_member_id
        description: optional files from the deleted member account will be transferred
          to this member
      responses:
        200:
          description: OK
      tags:
      - Remove