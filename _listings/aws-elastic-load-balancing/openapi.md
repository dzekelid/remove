swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
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
      description: Removes the specified tags from the specified resource.
      operationId: removeTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: ResourceArns.member.N
        description: The Amazon Resource Name (ARN) of the resource
        type: string
      - in: query
        name: TagKeys.member.N
        description: The tag keys for the tags to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags