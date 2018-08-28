swagger: "2.0"
x-collection-name: VictorOps
x-complete: 1
info:
  title: Victor Ops
  description: this-api-allows-you-to-interact-with-the-victorops-platform-in-various-ways--your-account-may-be-limitedto-a-total-number-of-api-calls-per-month--also-some-of-these-api-calls-have-rate-limits-note-in-this-documentation-when-creating-a-sample-curl-request-clicking-the-try-it-out-button-in-some-apiviewing-interfaces-the--in-an-email-address-may-be-encoded--please-note-that-the-rest-endpoints-will-notprocess-the-encoded-version--make-sure-that-the-encoded-character-40-is-changed-to-its-unencoded-form-beforesubmitting-the-curl-request-
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/team/{team}:
    delete:
      summary: Remove a team
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.delete
      x-api-path-slug: apipublicv1teamteam-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
  /api-public/v1/team/{team}/members/{user}:
    delete:
      summary: Remove a team member
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.user.delete
      x-api-path-slug: apipublicv1teamteammembersuser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      - in: path
        name: user
        description: The team member username
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Members
      - User
  /api-public/v1/user/{user}:
    delete:
      summary: Remove a user
      description: |-
        Remove a user from your organization

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.user.user.delete
      x-api-path-slug: apipublicv1useruser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user to be deleted
      responses:
        200:
          description: OK
      tags:
      - User
      - User