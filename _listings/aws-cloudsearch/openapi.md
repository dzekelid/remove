---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteExpression:
    get:
      summary: Delete Expression
      description: "Removes an \n  Expression\n  from the search domain."
      operationId: DeleteExpression
      x-api-path-slug: actiondeleteexpression-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: ExpressionName
        description: The name of the                         Expression                      to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Expressions
  /?Action=DeleteIndexField:
    get:
      summary: Delete Index Field
      description: "Removes an \n  IndexField\n  from the search domain."
      operationId: DeleteIndexField
      x-api-path-slug: actiondeleteindexfield-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: IndexFieldName
        description: The name of the index field your want to remove from the domains
          indexing options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: |-
        Removes the specified resource tags
         from an Amazon ES domain.
      operationId: RemoveTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: Base
        description: An error occurred while                  processing the request
        type: string
      - in: query
        name: InternalException
        description: The                  processing of the request failed because
          of an internal service error
        type: string
      - in: query
        name: ValidationException
        description: The                  request contains invalid input or is missing
          required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
---