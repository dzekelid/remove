---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Remove public certificate
  description: |-
    Delete the current public certificate being used with your SAML configuration. This will also disable encryption for SAML on your system as this certificate is required for that.
    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{team_id}/members/{user_id}:
    delete:
      summary: Remove user from team
      description: |-
        Delete the team member object for a user, effectively removing them from a team.
        ##### Permissions
        Must be logged in as the user or have the `remove_user_from_team` permission.
      operationId: delete-the-team-member-object-for-a-user-effectively-removing-them-from-a-team-permissionsmust-be-lo
      x-api-path-slug: teamsteam-idmembersuser-id-delete
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Team
  /channels/{channel_id}/members/{user_id}:
    delete:
      summary: Remove user from channel
      description: |-
        Delete a channel member, effectively removing them from a channel.
        ##### Permissions
        `manage_public_channel_members` permission if the channel is public.
        `manage_private_channel_members` permission if the channel is private.
      operationId: delete-a-channel-member-effectively-removing-them-from-a-channel-permissionsmanage-public-channel-me
      x-api-path-slug: channelschannel-idmembersuser-id-delete
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Channel
  /license:
    delete:
      summary: Remove license file
      description: |-
        Remove the license file from the server. This will disable all enterprise features.

        __Minimum server version__: 4.0

        ##### Permissions
        Must have `manage_system` permission.
      operationId: remove-the-license-file-from-the-server-this-will-disable-all-enterprise-features-minimum-server-ver
      x-api-path-slug: license-delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - License
      - File
  /saml/certificate/idp:
    delete:
      summary: Remove IDP certificate
      description: |-
        Delete the current IDP certificate being used with your SAML configuration. This will also disable SAML on your system as this certificate is required for SAML.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: delete-the-current-idp-certificate-being-used-with-your-saml-configuration-this-will-also-disable-sa
      x-api-path-slug: samlcertificateidp-delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - IDP
      - Certificate
  /saml/certificate/public:
    delete:
      summary: Remove public certificate
      description: |-
        Delete the current public certificate being used with your SAML configuration. This will also disable encryption for SAML on your system as this certificate is required for that.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: delete-the-current-public-certificate-being-used-with-your-saml-configuration-this-will-also-disable
      x-api-path-slug: samlcertificatepublic-delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Public
      - Certificate
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