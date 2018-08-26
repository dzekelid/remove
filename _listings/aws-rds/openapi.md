---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveRoleFromDBCluster:
    get:
      summary: Remove Role From D B Cluster
      description: Disassociates an Identity and Access Management (IAM) role from
        an Aurora DB cluster.
      operationId: removerolefromdbcluster
      x-api-path-slug: actionremoverolefromdbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to disassociate the IAM role rom
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the IAM role to disassociate
          from the Aurora DB cluster, for example        arn:aws:iam::123456789012:role/AuroraAccessRole
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=RemoveSourceIdentifierFromSubscription:
    get:
      summary: Remove Source Identifier From Subscription
      description: Removes a source identifier from an existing RDS event notification
        subscription.
      operationId: removesourceidentifierfromsubscription
      x-api-path-slug: actionremovesourceidentifierfromsubscription-get
      parameters:
      - in: query
        name: SourceIdentifier
        description: The source identifier to be removed from the subscription, such
          as the DB instance identifier             for a DB instance or the name
          of a security group
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to remove a source identifier from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes metadata tags from an Amazon RDS resource.
      operationId: removetagsfromresource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon RDS resource the tags will be removed from
        type: string
      - in: query
        name: TagKeys.member.N
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
---