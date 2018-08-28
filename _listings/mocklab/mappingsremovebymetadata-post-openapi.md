---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 0
info:
  title: MockLab Post Mappings Remove By Metadata
  version: 1.0.0
  description: Remove stubs by matching on their metadata
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mappings/remove-by-metadata:
    post:
      summary: Post Mappings Remove By Metadata
      description: Remove stubs by matching on their metadata
      operationId: postMappingsRemoveByMetadata
      x-api-path-slug: mappingsremovebymetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Remove
      - Metadata
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