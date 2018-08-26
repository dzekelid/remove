---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
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
---