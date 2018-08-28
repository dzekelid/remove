---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Delete Account
  description: Remove subscription from account. JSON with subscription details is
    sent. Can be performed only by system/admin.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/subscriptions/{subscriptionId}:
    delete:
      summary: Delete Account Subscriptions Subscriptionid
      description: 'Remove subscription from account. Roles: account/owner, system/admin.'
      operationId: removeSubscription
      x-api-path-slug: accountsubscriptionssubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
  /account/{id}:
    delete:
      summary: Delete Account
      description: Remove subscription from account. JSON with subscription details
        is sent. Can be performed only by system/admin.
      operationId: remove
      x-api-path-slug: accountid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
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