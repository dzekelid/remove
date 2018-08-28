---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Detach Principal Policy
  version: 1.0.0
  description: Removes the specified policy from the specified certificate.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachPrincipalPolicy:
    get:
      summary: Detach Principal Policy
      description: Removes the specified policy from the specified certificate.
      operationId: detachPrincipalPolicy
      x-api-path-slug: actiondetachprincipalpolicy-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy to detach
        type: string
      - in: query
        name: principal
        description: The principal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Policies
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