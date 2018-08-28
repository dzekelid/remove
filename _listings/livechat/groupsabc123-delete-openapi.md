---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Remove a group
  description: Removes a group with the given GROUP_ID.
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /goals/ABC123:
    delete:
      summary: Remove a goal
      description: Removes a goal with the given GOAL_ID.
      operationId: GoalsABC123Delete
      x-api-path-slug: goalsabc123-delete
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Goal
  /greetings/ABC123:
    delete:
      summary: Remove a greeting
      description: Removes a greeting.
      operationId: GreetingsABC123Delete
      x-api-path-slug: greetingsabc123-delete
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Greeting
  /agents/john@public.com:
    delete:
      summary: Remove an agent
      description: Removes an agent.
      operationId: AgentsJohnPublicComDelete
      x-api-path-slug: agentsjohnpublic-com-delete
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Agent
  /groups/ABC123:
    delete:
      summary: Remove a group
      description: Removes a group with the given GROUP_ID.
      operationId: GroupsABC123Delete2
      x-api-path-slug: groupsabc123-delete
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
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