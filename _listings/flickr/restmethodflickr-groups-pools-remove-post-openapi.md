---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Groups Pools Remove
  description: Remove a photo from a group pool.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.favorites.remove:
    get:
      summary: Favorites Remove
      description: Adds a photo to a user's favorites list.
      operationId: getRestMethodFlickr.favorites.remove
      x-api-path-slug: restmethodflickr-favorites-remove-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to remove to the users favorites
      responses:
        200:
          description: OK
      tags:
      - Favorites
      - Remove
  /rest/?method=flickr.groups.pools.remove:
    post:
      summary: Groups Pools Remove
      description: Remove a photo from a group pool.
      operationId: postRestMethodFlickr.groups.pools.remove
      x-api-path-slug: restmethodflickr-groups-pools-remove-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: group_id
        description: The NSID of the group whos pool the photo is to removed from
      - in: query
        name: photo_id
        description: The id of the photo to remove from the group pool
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Pools
      - Remove
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