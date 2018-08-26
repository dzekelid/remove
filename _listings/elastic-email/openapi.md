---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 1
info:
  title: Elastic Email SMTP API
  description: api-for-sending-and-management-email-
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
---