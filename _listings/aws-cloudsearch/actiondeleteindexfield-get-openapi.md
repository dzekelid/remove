---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch Delete Index Field
  version: 1.0.0
  description: "Removes an \n  IndexField\n  from the search domain."
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