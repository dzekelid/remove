---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Remove Role From Instance Profile
  version: 1.0.0
  description: Removes the specified IAM role from the specified EC2 instance profile.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachGroupPolicy:
    get:
      summary: Detach Group Policy
      description: Removes the specified managed policy from the specified IAM group.
      operationId: detachGroupPolicy
      x-api-path-slug: actiondetachgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) of the IAM group to detach
          the policy      from
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=DetachRolePolicy:
    get:
      summary: Detach Role Policy
      description: Removes the specified managed policy from the specified role.
      operationId: detachRolePolicy
      x-api-path-slug: actiondetachrolepolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      - in: query
        name: RoleName
        description: The name (friendly name, not ARN) of the IAM role to detach the
          policy      from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=DetachUserPolicy:
    get:
      summary: Detach User Policy
      description: Removes the specified managed policy from the specified user.
      operationId: detachUserPolicy
      x-api-path-slug: actiondetachuserpolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      - in: query
        name: UserName
        description: The name (friendly name, not ARN) of the IAM user to detach the
          policy      from
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Policies
  /?Action=RemoveClientIDFromOpenIDConnectProvider:
    get:
      summary: Remove Client I D From Open I D Connect Provider
      description: |-
        Removes the specified client ID (also known as audience) from the list of client IDs
              registered for the specified IAM OpenID Connect (OIDC) provider resource object.
      operationId: removeClientIDFromOpenIDConnectProvider
      x-api-path-slug: actionremoveclientidfromopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientID
        description: The client ID (also known as audience) to remove from the IAM
          OIDC provider resource
        type: string
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          to remove the client      ID from
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=RemoveRoleFromInstanceProfile:
    get:
      summary: Remove Role From Instance Profile
      description: Removes the specified IAM role from the specified EC2 instance
        profile.
      operationId: removeRoleFromInstanceProfile
      x-api-path-slug: actionremoverolefrominstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to update
        type: string
      - in: query
        name: RoleName
        description: The name of the role to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role From Instance Profiles
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