---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Remove watcher
  description: Removes the user from the issue's watcher list.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/filter/{id}/favourite:
    delete:
      summary: Remove filter as favorite
      description: Removes a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
        and permission to view the filter.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.deleteFavouriteForFilter_delete
      x-api-path-slug: api2filteridfavourite-delete
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: path
        name: id
        description: The ID of the filter
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Filter
      - As
      - Favorite
  /api/2/group:
    delete:
      summary: Remove group
      description: |-
        Deletes a group.

        **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.GroupResource.removeGroup_delete
      x-api-path-slug: api2group-delete
      parameters:
      - in: query
        name: groupname
        description: The name of the group
      - in: query
        name: swapGroup
        description: The group to transfer restrictions to
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
  /api/2/group/user:
    delete:
      summary: Remove user from group
      description: Removes a user from a group. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
        _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.GroupResource.removeUserFromGroup_delete
      x-api-path-slug: api2groupuser-delete
      parameters:
      - in: query
        name: accountid
        description: The account id of the user to remove
      - in: header
        name: force-account-id
      - in: query
        name: groupname
        description: The name of the group
      - in: query
        name: username
        description: The username of the user to remove
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Group
  /api/2/issue/{issueIdOrKey}/votes:
    delete:
      summary: Remove vote
      description: Removes a current user's vote from an issue (aka "unvote").
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.removeVote_delete
      x-api-path-slug: api2issueissueidorkeyvotes-delete
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue that current user unvotes
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Vote
  /api/2/issue/{issueIdOrKey}/watchers:
    delete:
      summary: Remove watcher
      description: Removes the user from the issue's watcher list.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.removeWatcher_delete
      x-api-path-slug: api2issueissueidorkeywatchers-delete
      parameters:
      - in: query
        name: accountId
        description: Account ID of the user to be removed from the watcher list
      - in: header
        name: force-account-id
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be updated
      - in: query
        name: username
        description: Name of the user to be removed from the watcher list
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Watcher
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