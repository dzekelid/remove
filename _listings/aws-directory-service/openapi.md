---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeregisterEventTopic:
    get:
      summary: Deregister Event Topic
      description: Removes the specified directory as a publisher to the specified
        SNS topic.
      operationId: deregisterEventTopic
      x-api-path-slug: actionderegistereventtopic-get
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID to remove as a publisher
        type: string
      - in: query
        name: TopicName
        description: The name of the SNS topic from which to remove the directory
          as a publisher
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Topics
  /?Action=RemoveIpRoutes:
    get:
      summary: Remove Ip Routes
      description: Removes IP address blocks from a directory.
      operationId: removeIpRoutes
      x-api-path-slug: actionremoveiproutes-get
      parameters:
      - in: query
        name: CidrIps
        description: IP address blocks that you want to remove
        type: string
      - in: query
        name: DirectoryId
        description: Identifier (ID) of the directory from which you want to remove
          the IP addresses
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address Routes
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes tags from a directory.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: Identifier (ID) of the directory from which to remove the tag
        type: string
      - in: query
        name: TagKeys
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
---