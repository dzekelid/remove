swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 1
info:
  title: AWS CloudFront API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UntagResource:
    get:
      summary: Untag Resource
      description: Remove tags from a CloudFront resource.
      operationId: untagResource
      x-api-path-slug: actionuntagresource-get
      parameters:
      - in: query
        name: Device
        description: The device name to expose to the instance (for example, /dev/sdh
          or        xvdh)
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      - in: query
        name: VolumeId
        description: The ID of the EBS volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Untag
      - Resource