swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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
  /rest/items/{id}/variations/{variationId}/variation_categories/{catId}:
    delete:
      summary: Remove a category from a variation
      description: Deletes the link between a category and a variation.
      operationId: deleteRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-delete
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Category
      - From
      - Variation
  /rest/plugin_sets/{setId}/plugins/{pluginId}:
    delete:
      summary: Remove a plugin from a set
      description: |-
        Removes a plugin from a set and deletes all plugin files. Response content will be 'true' if the deletion was successful,
        'false' if not. If no plugin set with the given id can be found or the plugin is not associated to the set, a 404 will be returned.
      operationId: deleteRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-delete
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Plugin
      - From
      - Set
  /rest/storage/frontend/file:
    delete:
      summary: Remove a single object from frontend storage.
      description: Remove a single object from frontend storage..
      operationId: deleteRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-delete
      parameters:
      - in: query
        name: key
        description: The key of the object to delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Single
      - Object
      - From
      - Frontend
      - Storage