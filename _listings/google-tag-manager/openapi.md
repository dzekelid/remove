---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 1
info:
  title: Tag Manager
  description: accesses-tag-manager-accounts-and-containers-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/permissions/{permissionId}:
    delete:
      summary: Remove User
      description: Removes a user from the account, revoking access to it and all
        of its containers.
      operationId: tagmanager.accounts.permissions.delete
      x-api-path-slug: accountsaccountidpermissionspermissionid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: permissionId
        description: The GTM User ID
      responses:
        200:
          description: OK
      tags:
      - User
---