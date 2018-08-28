swagger: "2.0"
x-collection-name: Reddit
x-complete: 1
info:
  title: Reddit
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /remove:
    post&nbsp;:
      summary: Add Remove
      description: Remove a link, comment, or modmail message.
      operationId: post&nbsp;Remove
      x-api-path-slug: remove-postnbsp
      parameters:
      - in: query
        name: id
        description: fullname of a thing
        type: string
      - in: query
        name: spam
        description: boolean value
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove