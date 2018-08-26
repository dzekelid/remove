---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /addons/{id}:
    delete:
      summary: Delete an add-on
      description: Remove an existing add-on.
      operationId: remove-an-existing-addon
      x-api-path-slug: addonsid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - AddOns
---