---
swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 1
info:
  title: AWS Data Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: Removes existing tags from the specified pipeline.
      operationId: removeTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: tagKeys
        description: The keys of the tags to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
---