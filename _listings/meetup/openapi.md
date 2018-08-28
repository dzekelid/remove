swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/topics:
    delete:
      summary: Group Topics Remove
      description: Disassociates topics with a given Meetup group. Limited to organizers
        of the group. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
        permission.
      operationId: groups
      x-api-path-slug: urlnametopics-delete
      parameters:
      - in: query
        name: topic_id
        description: Comma-delimited list of topic ids to disassociate with group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos