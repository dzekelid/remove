---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Remove User
  description: Removes a user from the account, revoking access to it and all of its
    containers.
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