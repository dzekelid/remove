---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Remove a bundle component
  description: Removes a component from a bundle. The bundle ID must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/{id}/variations/{variationId}/variation_bundles/{bundleId}:
    delete:
      summary: Remove a bundle component
      description: Removes a component from a bundle. The bundle ID must be specified.
      operationId: deleteRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-delete
      parameters:
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Bundle
      - Component
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