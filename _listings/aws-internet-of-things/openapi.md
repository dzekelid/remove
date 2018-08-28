swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
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