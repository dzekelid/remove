---
swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 0
info:
  title: AWS WAF API Disassociate Web ACL
  version: 1.0.0
  description: 'Service: AWS WAF RegionalRemoves a web ACL from the specified resource.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisassociateWebACL:
    get:
      summary: Disassociate Web ACL
      description: 'Service: AWS WAF RegionalRemoves a web ACL from the specified
        resource.'
      operationId: disassociateWebACL
      x-api-path-slug: actiondisassociatewebacl-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource from which the
          web ACL is being removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
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