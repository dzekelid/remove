---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Conversations API Delete a message
  description: Delete a message.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conversations/{id}/remove_messages:
    post:
      summary: Delete a message
      description: Delete a message.
      operationId: delete-a-message
      x-api-path-slug: conversationsidremove-messages-post
      parameters:
      - in: query
        name: remove[]
        description: Array of message ids to be deleted
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
      - Remove
      - Messages
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