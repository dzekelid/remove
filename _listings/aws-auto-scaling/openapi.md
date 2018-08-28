swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DetachInstances:
    get:
      summary: Detach Instances
      description: Removes one or more instances from the specified Auto Scaling group.
      operationId: detachInstances
      x-api-path-slug: actiondetachinstances-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If True, the Auto Scaling group decrements the desired capacity
          value by the number of instances detached
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instances