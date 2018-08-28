---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Delete workflow scheme issue type
  description: Remove the specified issue type mapping from the scheme.
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
  /content/{id}/label:
    delete:
      summary: Remove label from content using query parameter
      description: "Removes a label from a piece of content. This is similar to \n[Remove
        label from content](#api-content-id-label-label-delete) \nexcept that the
        label name is specified via a query parameter. \n\nUse this method if the
        label name has \"/\" characters, as \n[Remove label from content using query
        parameter](#api-content-id-label-delete) \ndoes not accept \"/\" characters
        for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentLabelsResource.removeLabelFromContentUsing
      x-api-path-slug: contentidlabel-delete
      parameters:
      - in: path
        name: id
        description: The ID of the content that the label will be removed from
      - in: query
        name: name
        description: The name of the label to be removed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Label
      - From
      - Content
      - Using
      - Query
      - Parameter
  /content/{id}/label/{label}:
    delete:
      summary: Remove label from content
      description: "Removes a label from a piece of content. This is similar to \n[Remove
        label from content using query parameter](#api-content-id-label-delete) \nexcept
        that the label name is specified via a path parameter. \n\nUse this method
        if the label name does not have \"/\" characters, as the path \nparameter
        does not accept \"/\" characters for security reasons. Otherwise, \nuse [Remove
        label from content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to update the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentLabelsResource.removeLabelFromContent_dele
      x-api-path-slug: contentidlabellabel-delete
      parameters:
      - in: path
        name: id
        description: The ID of the content that the label will be removed from
      - in: path
        name: label
        description: The name of the label to be removed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Label
      - From
      - Content
  /content/{id}/restriction/byOperation/{operationKey}/group/{groupName}:
    delete:
      summary: Remove group from content restriction
      description: "Removes a group from a content restriction. That is, remove read
        or update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to edit the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentRestrictionResource.removeGroupFromContent
      x-api-path-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-delete
      parameters:
      - in: path
        name: groupName
        description: The name of the group to remove from the content restriction
      - in: path
        name: id
        description: The ID of the content that the restriction applies to
      - in: path
        name: operationKey
        description: The operation that the restriction applies to
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
      - From
      - Content
      - Restriction
  /content/{id}/restriction/byOperation/{operationKey}/user:
    delete:
      summary: Remove user from content restriction
      description: "Removes a group from a content restriction. That is, remove read
        or update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to edit the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentRestrictionResource.removeUserFromContentR
      x-api-path-slug: contentidrestrictionbyoperationoperationkeyuser-delete
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user to remove from the content restriction
      - in: path
        name: id
        description: The ID of the content that the restriction applies to
      - in: query
        name: key
        description: The key of the user to remove from the content restriction
      - in: path
        name: operationKey
        description: The operation that the restriction applies to
      - in: query
        name: userName
        description: The username of the user to remove from the content restriction
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Content
      - Restriction
  /template/{contentTemplateId}:
    delete:
      summary: Remove template
      description: "Deletes a template. This results in different actions depending
        on the \ntype of template:\n\n- If the template is a content template, it
        is deleted.\n- If the template is a modified space-level blueprint template,
        it reverts \nto the template inherited from the global-level blueprint template.\n-
        If the template is a modified global-level blueprint template, it reverts
        \nto the default global-level blueprint template.\n\n Note, unmodified blueprint
        templates cannot be deleted."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.removeTemplate_delete
      x-api-path-slug: templatecontenttemplateid-delete
      parameters:
      - in: path
        name: contentTemplateId
        description: The ID of the template to be deleted
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Template
  /user/watch/content/{contentId}:
    delete:
      summary: Remove content watcher
      description: "Removes a user as a watcher from a piece of content. Choose the
        user by \ndoing one of the following:\n\n- Specify a user via a query parameter:
        Use the `username`, `key`, or `accountId` \nto identify the user. The user
        making the request must be a Confluence administrator.\n- Do not specify a
        user: The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.removeContentWatcher_delete
      x-api-path-slug: userwatchcontentcontentid-delete
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be removed as a watcher
      - in: path
        name: contentId
        description: The ID of the content to remove the watcher from
      - in: query
        name: key
        description: The `key` of the user that will be removed as a watcher
      - in: query
        name: username
        description: The `username` of the user that will be removed as a watcher
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Content
      - Watcher
  /user/watch/label/{labelName}:
    delete:
      summary: Remove label watcher
      description: "Removes a user as a watcher from a label. Choose the user by doing
        one of \nthe following:\n\n- Specify a user via a query parameter: Use the
        `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.removeLabelWatcher_delete
      x-api-path-slug: userwatchlabellabelname-delete
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be removed as a watcher
      - in: query
        name: key
        description: The `key` of the user that will be removed as a watcher
      - in: path
        name: labelName
        description: The name of the label to remove the watcher from
      - in: query
        name: username
        description: The `username` of the user that will be removed as a watcher
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Label
      - Watcher
  /user/watch/space/{spaceKey}:
    delete:
      summary: Remove space watch
      description: "Removes a user as a watcher from a space. Choose the user by doing
        one of \nthe following:\n\n- Specify a user via a query parameter: Use the
        `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.removeSpaceWatch_delete
      x-api-path-slug: userwatchspacespacekey-delete
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be removed as a watcher
      - in: query
        name: key
        description: The `key` of the user that will be removed as a watcher
      - in: path
        name: spaceKey
        description: The key of the space to remove the watcher from
      - in: query
        name: username
        description: The `username` of the user that will be removed as a watcher
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Space
      - Watch
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
  /api/2/mypreferences:
    delete:
      summary: Remove preference
      description: Removes preference of the currently logged in user. Preference
        key must be provided as input parameters (key).
      operationId: com.atlassian.jira.rest.v2.preference.CurrentUserPreferencesResource.removePreference_delete
      x-api-path-slug: api2mypreferences-delete
      parameters:
      - in: query
        name: key
        description: \- key of the preference to be removed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Preference
  /api/2/projectCategory/{id}:
    delete:
      summary: Remove project category
      description: Delete a project category.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectCategoryResource.removeProjectCategory_delete
      x-api-path-slug: api2projectcategoryid-delete
      parameters:
      - in: path
        name: id
        description: Id of the project category to delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Project
      - Category
  /api/2/screens/{screenId}/tabs/{tabId}/fields/{id}:
    delete:
      summary: Remove screen tab field
      description: Removes field from given tab
      operationId: com.atlassian.jira.rest.v2.issue.ScreensResource.removeScreenTabField_delete
      x-api-path-slug: api2screensscreenidtabstabidfieldsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: screenId
        description: id of screen
      - in: path
        name: tabId
        description: id of tab
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Screen
      - Tab
      - Field
  /api/2/comment/{commentId}/properties/{propertyKey}:
    delete:
      summary: Delete comment property
      description: Removes the property from the comment identified by the key or
        by the id. Ths user removing the property is required to have permissions
        to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.deleteCommentProperty_delete
      x-api-path-slug: api2commentcommentidpropertiespropertykey-delete
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be removed
      - in: path
        name: propertyKey
        description: the key of the property to remove
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
  /api/2/issue/{issueIdOrKey}/properties/{propertyKey}:
    delete:
      summary: Delete issue property
      description: Removes the property from the issue identified by the key or by
        the id. Ths user removing the property is required to have permissions to
        edit the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.deleteIssueProperty_delete
      x-api-path-slug: api2issueissueidorkeypropertiespropertykey-delete
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue from which the property will be removed
      - in: path
        name: propertyKey
        description: the key of the property to remove
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Property
  /api/2/issue/{issueIdOrKey}/worklog/{worklogId}/properties/{propertyKey}:
    delete:
      summary: Delete worklog property
      description: Removes the property from the worklog identified by the key or
        by the id. Ths user removing the property is required to have permissions
        to administer the worklog.
      operationId: com.atlassian.jira.rest.v2.issue.WorklogPropertyResource.deleteWorklogProperty_delete
      x-api-path-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
      parameters:
      - in: path
        name: issueIdOrKey
      - in: path
        name: propertyKey
        description: the key of the property to remove
      - in: path
        name: worklogId
        description: the worklog from which the property will be removed
      responses:
        200:
          description: OK
      tags:
      - Worklog
      - Property
  /api/2/project/{projectIdOrKey}/properties/{propertyKey}:
    delete:
      summary: Delete project property
      description: |-
        Removes the [property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) from the project.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectPropertyResource.deleteProjectProperty_delete
      x-api-path-slug: api2projectprojectidorkeypropertiespropertykey-delete
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: path
        name: propertyKey
        description: The project property key
      responses:
        200:
          description: OK
      tags:
      - Project
      - Property
  /api/2/role/{id}/actors:
    delete:
      summary: Delete default actors from project role
      description: |-
        Removes [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) from the project role. You may remove either a group or user, but you cannot remove a group and a user in the same request.

        Changing a project role's default actors does not affect project role members for projects already created.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.deleteProjectRoleActorsFromRole_delete
      x-api-path-slug: api2roleidactors-delete
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: group
        description: The group name of the group to be removed as a default actor
      - in: path
        name: id
        description: The ID of the project role
      - in: query
        name: user
        description: The user account ID of the user to remove as a default actor
      responses:
        200:
          description: OK
      tags:
      - Default
      - Actors
      - From
      - Project
      - Role
  /api/2/workflowscheme/{id}/default:
    delete:
      summary: Delete default workflow
      description: Remove the default workflow from the passed workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteDefaultWorkflow_delete
      x-api-path-slug: api2workflowschemeiddefault-delete
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: query
        name: updateDraftIfNeeded
        description: when true will create and return a draft when the workflow scheme
          cannot be edited (e
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
  /api/2/workflowscheme/{id}/draft/default:
    delete:
      summary: Delete draft default workflow
      description: Remove the default workflow from the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteDraftDefaultWorkflow_de
      x-api-path-slug: api2workflowschemeiddraftdefault-delete
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
  /api/2/workflowscheme/{id}/draft/issuetype/{issueType}:
    delete:
      summary: Delete workflow scheme draft issue type
      description: Remove the specified issue type mapping from the draft scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteWorkflowSchemeDraftIssu
      x-api-path-slug: api2workflowschemeiddraftissuetypeissuetype-delete
      parameters:
      - in: path
        name: id
        description: the parent of the draft scheme
      - in: path
        name: issueType
        description: the issue type to remove
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
      - Issue
      - Type
  /api/2/workflowscheme/{id}/issuetype/{issueType}:
    delete:
      summary: Delete workflow scheme issue type
      description: Remove the specified issue type mapping from the scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteWorkflowSchemeIssueType
      x-api-path-slug: api2workflowschemeidissuetypeissuetype-delete
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: path
        name: issueType
        description: the issue type to remove
      - in: query
        name: updateDraftIfNeeded
        description: when true will create and return a draft when the workflow scheme
          cannot be edited (e
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Issue
      - Type
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