---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Remove Cards from Deck
  version: 1.0.0
  description: Remove cards from deck.
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/analytic/execution/async/{requestId}:
    delete:
      summary: Cleanup analytic execution result by request id.
      description: Removes the analytic execution result from the cache. It is highly
        recommended to clean your old result data to have room for future result data.
      operationId: clearAnalyticExecutionResult
      x-api-path-slug: apiv1analyticexecutionasyncrequestid-delete
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Predix-Zone-Id
      - in: path
        name: requestId
      responses:
        2:
          description: Successful response
      tags:
      - Cleanup
      - Analytic
      - Execution
      - Result
      - By
      - Request
      - Id
  /v1/group/removeFromGroup:
    post:
      summary: Remove Object from Group
      description: Remove Object from Group.
      operationId: leaveGroup
      x-api-path-slug: v1groupremovefromgroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Object
      - From
      - Group
  /decks/{id}/cards/remove:
    post:
      summary: Remove Cards from Deck
      description: Remove cards from deck.
      operationId: postDecksCardsRemove
      x-api-path-slug: decksidcardsremove-post
      parameters:
      - in: body
        name: cardIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Cards
      - From
      - Deck
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