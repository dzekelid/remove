swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RevokeSnapshotAccess:
    get:
      summary: Revoke Snapshot Access
      description: |-
        Removes the ability of the specified AWS customer account to restore the specified
                    snapshot.
      operationId: revokeSnapshotAccess
      x-api-path-slug: actionrevokesnapshotaccess-get
      parameters:
      - in: query
        name: AccountWithRestoreAccess
        description: The identifier of the AWS customer account that can no longer
          restore the specified            snapshot
        type: string
      - in: query
        name: SnapshotClusterIdentifier
        description: The identifier of the cluster the snapshot was created from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier of the snapshot that the account can no longer
          access
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots