---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Deregister Patch Baseline For Patch Group
  version: 1.0.0
  description: Removes a patch group from a patch baseline.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes all tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to remove tags
        type: string
      - in: query
        name: ResourceType
        description: The type of resource of which you want to remove a tag
        type: string
      - in: query
        name: TagKeys
        description: Tag keys that you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Tags
      - From
      - Resource
  /?Action=DeregisterManagedInstance:
    get:
      summary: Deregister Managed Instance
      description: Removes the server or virtual machine from the list of registered
        servers.
      operationId: deregisterManagedInstance
      x-api-path-slug: actionderegistermanagedinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID assigned to the managed instance when you registered it
          using the activation   process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Managed
      - Instance
  /?Action=DeregisterPatchBaselineForPatchGroup:
    get:
      summary: Deregister Patch Baseline For Patch Group
      description: Removes a patch group from a patch baseline.
      operationId: deregisterPatchBaselineForPatchGroup
      x-api-path-slug: actionderegisterpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to deregister the patch group from
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group that should be deregistered from
          the patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - BaselineGroup
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