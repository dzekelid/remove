---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API Remove Auto Scaling Policy
  version: 1.0.0
  description: Removes an automatic scaling policy from a specified instance group
    within an EMR cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveAutoScalingPolicy:
    get:
      summary: Remove Auto Scaling Policy
      description: Removes an automatic scaling policy from a specified instance group
        within an EMR cluster.
      operationId: removeAutoScalingPolicy
      x-api-path-slug: actionremoveautoscalingpolicy-get
      parameters:
      - in: query
        name: ClusterId
        description: Specifies the ID of a cluster
        type: string
      - in: query
        name: InstanceGroupId
        description: Specifies the ID of the instance group to which the scaling policy
          is applied
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Policies
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