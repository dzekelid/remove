swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 1
info:
  title: AWS Shield API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteSubscription:
    get:
      summary: Delete Subscription
      description: Removes AWS Shield Advanced from an account.
      operationId: deleteSubscription
      x-api-path-slug: actiondeletesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection