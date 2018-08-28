swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
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
  /account/{id}/attribute:
    delete:
      summary: Delete Account Attribute
      description: Remove attribute from an account. Attribute name is used as a quary
        parameter. For this API request account/owner, system/admin or system/manager
        role is required
      operationId: removeAttribute
      x-api-path-slug: accountidattribute-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: name
        description: Attribute name to be removed
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Attribute
  /account/{id}/members/{userid}:
    delete:
      summary: Delete Account Members User
      description: Remove user from a specific account. This API call requires account/owner,
        system/admin or system/manager role.
      operationId: removeMember
      x-api-path-slug: accountidmembersuserid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
      - Userid