---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Remove Tags From Resource
  version: 1.0.0
  description: Removes all tags from the specified resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes all tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to remove tags
        type: string
      - in: query
        name: ResourceType
        description: The type of resource of which you want to remove a tag
        type: string
      - in: query
        name: TagKeys
        description: Tag keys that you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Tags
      - From
      - Resource
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