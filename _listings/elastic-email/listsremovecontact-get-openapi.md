---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 0
info:
  title: Elastic Email SMTP API Remove Existing Subscriber From List
  description: Remove Existing Subscriber From List
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  lists/remove-contact:
    get:
      summary: Remove Existing Subscriber From List
      description: Remove Existing Subscriber From List
      operationId: getListsRemoveContact
      x-api-path-slug: listsremovecontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to remove subscriber from (separate by
          semi-colon to remove from multiple lists)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Remove
      - Contact
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