---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Remove
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Remove label from content using query parameter
  x-api-slug: contentidlabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content](#api-content-id-label-label-delete) \nexcept that the label
    name is specified via a query parameter. \n\nUse this method if the label name
    has \"/\" characters, as \n[Remove label from content using query parameter](#api-content-id-label-delete)
    \ndoes not accept \"/\" characters for the label name.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidlabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidlabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label from content
  x-api-slug: contentidlabellabel-delete
  description: "Removes a label from a piece of content. This is similar to \n[Remove
    label from content using query parameter](#api-content-id-label-delete) \nexcept
    that the label name is specified via a path parameter. \n\nUse this method if
    the label name does not have \"/\" characters, as the path \nparameter does not
    accept \"/\" characters for security reasons. Otherwise, \nuse [Remove label from
    content using query parameter](#api-content-id-label-delete).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to update the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidlabellabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidlabellabel-delete-openapi.md
- name: The Confluence Cloud REST API - Remove group from content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-delete
  description: "Removes a group from a content restriction. That is, remove read or
    update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-delete-openapi.md
- name: The Confluence Cloud REST API - Remove user from content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeyuser-delete
  description: "Removes a group from a content restriction. That is, remove read or
    update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeyuser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeyuser-delete-openapi.md
- name: The Confluence Cloud REST API - Remove template
  x-api-slug: templatecontenttemplateid-delete
  description: "Deletes a template. This results in different actions depending on
    the \ntype of template:\n\n- If the template is a content template, it is deleted.\n-
    If the template is a modified space-level blueprint template, it reverts \nto
    the template inherited from the global-level blueprint template.\n- If the template
    is a modified global-level blueprint template, it reverts \nto the default global-level
    blueprint template.\n\n Note, unmodified blueprint templates cannot be deleted."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/templatecontenttemplateid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/templatecontenttemplateid-delete-openapi.md
- name: The Confluence Cloud REST API - Remove content watcher
  x-api-slug: userwatchcontentcontentid-delete
  description: "Removes a user as a watcher from a piece of content. Choose the user
    by \ndoing one of the following:\n\n- Specify a user via a query parameter: Use
    the `username`, `key`, or `accountId` \nto identify the user. The user making
    the request must be a Confluence administrator.\n- Do not specify a user: The
    currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/userwatchcontentcontentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/userwatchcontentcontentid-delete-openapi.md
- name: The Confluence Cloud REST API - Remove label watcher
  x-api-slug: userwatchlabellabelname-delete
  description: "Removes a user as a watcher from a label. Choose the user by doing
    one of \nthe following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/userwatchlabellabelname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/userwatchlabellabelname-delete-openapi.md
- name: The Confluence Cloud REST API - Remove space watch
  x-api-slug: userwatchspacespacekey-delete
  description: "Removes a user as a watcher from a space. Choose the user by doing
    one of \nthe following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/userwatchspacespacekey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/userwatchspacespacekey-delete-openapi.md
- name: Jira Cloud REST API - Remove filter as favorite
  x-api-slug: api2filteridfavourite-delete
  description: Removes a filter as a favorite for the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
    and permission to view the filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2filteridfavourite-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2filteridfavourite-delete-openapi.md
- name: Jira Cloud REST API - Remove group
  x-api-slug: api2group-delete
  description: |-
    Deletes a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2group-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2group-delete-openapi.md
- name: Jira Cloud REST API - Remove user from group
  x-api-slug: api2groupuser-delete
  description: Removes a user from a group. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
    _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2groupuser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2groupuser-delete-openapi.md
- name: Jira Cloud REST API - Remove vote
  x-api-slug: api2issueissueidorkeyvotes-delete
  description: Removes a current user's vote from an issue (aka "unvote").
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeyvotes-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeyvotes-delete-openapi.md
- name: Jira Cloud REST API - Remove watcher
  x-api-slug: api2issueissueidorkeywatchers-delete
  description: Removes the user from the issue's watcher list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeywatchers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeywatchers-delete-openapi.md
- name: Jira Cloud REST API - Remove preference
  x-api-slug: api2mypreferences-delete
  description: Removes preference of the currently logged in user. Preference key
    must be provided as input parameters (key).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2mypreferences-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2mypreferences-delete-openapi.md
- name: Jira Cloud REST API - Remove project category
  x-api-slug: api2projectcategoryid-delete
  description: Delete a project category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2projectcategoryid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2projectcategoryid-delete-openapi.md
- name: Jira Cloud REST API - Remove screen tab field
  x-api-slug: api2screensscreenidtabstabidfieldsid-delete
  description: Removes field from given tab
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2screensscreenidtabstabidfieldsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2screensscreenidtabstabidfieldsid-delete-openapi.md
- name: Jira Cloud REST API - Delete comment property
  x-api-slug: api2commentcommentidpropertiespropertykey-delete
  description: Removes the property from the comment identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2commentcommentidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete issue property
  x-api-slug: api2issueissueidorkeypropertiespropertykey-delete
  description: Removes the property from the issue identified by the key or by the
    id. Ths user removing the property is required to have permissions to edit the
    issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete worklog property
  x-api-slug: api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete
  description: Removes the property from the worklog identified by the key or by the
    id. Ths user removing the property is required to have permissions to administer
    the worklog.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2issueissueidorkeyworklogworklogidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete project property
  x-api-slug: api2projectprojectidorkeypropertiespropertykey-delete
  description: |-
    Removes the [property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) from the project.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2projectprojectidorkeypropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete default actors from project role
  x-api-slug: api2roleidactors-delete
  description: |-
    Removes [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) from the project role. You may remove either a group or user, but you cannot remove a group and a user in the same request.

    Changing a project role's default actors does not affect project role members for projects already created.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2roleidactors-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2roleidactors-delete-openapi.md
- name: Jira Cloud REST API - Delete default workflow
  x-api-slug: api2workflowschemeiddefault-delete
  description: Remove the default workflow from the passed workflow scheme.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeiddefault-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeiddefault-delete-openapi.md
- name: Jira Cloud REST API - Delete draft default workflow
  x-api-slug: api2workflowschemeiddraftdefault-delete
  description: Remove the default workflow from the passed draft workflow scheme.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeiddraftdefault-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeiddraftdefault-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow scheme draft issue type
  x-api-slug: api2workflowschemeiddraftissuetypeissuetype-delete
  description: Remove the specified issue type mapping from the draft scheme.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeiddraftissuetypeissuetype-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeiddraftissuetypeissuetype-delete-openapi.md
- name: Jira Cloud REST API - Delete workflow scheme issue type
  x-api-slug: api2workflowschemeidissuetypeissuetype-delete
  description: Remove the specified issue type mapping from the scheme.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeidissuetypeissuetype-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/remove/master/_listings/atlassian/api2workflowschemeidissuetypeissuetype-delete-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---