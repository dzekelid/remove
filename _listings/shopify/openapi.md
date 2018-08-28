swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/products/9579007950.json:
    delete:
      summary: Remove a product from the shop
      description: Remove a product from the shop.
      operationId: deleteAdminProducts9579007950.json
      x-api-path-slug: adminproducts9579007950-json-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Product
      - From
      - Shop
  /admin/themes/110163843/assets.json:
    delete:
      summary: Remove assets from your shop
      description: Remove assets from your shop.
      operationId: deleteAdminThemes110163843Assets.json
      x-api-path-slug: adminthemes110163843assets-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Assets
      - From
      - Your
      - Shop
  /admin/comments/2941387470/remove.json:
    post:
      summary: Remove a comment
      description: Remove a comment.
      operationId: postAdminComments2941387470Remove.json
      x-api-path-slug: admincomments2941387470remove-json-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Comment
  /admin/customers/5438892686.json:
    delete:
      summary: Remove an existing customer
      description: Remove an existing customer.
      operationId: deleteAdminCustomers5438892686.json
      x-api-path-slug: admincustomers5438892686-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Existing
      - Customer
  /admin/collects/921728736.json:
    delete:
      summary: Remove a product from a collection
      description: Remove a product from a collection.
      operationId: deleteAdminCollects921728736.json
      x-api-path-slug: admincollects921728736-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Product
      - From
      - Collection
  /admin/script_tags/108074126.json:
    delete:
      summary: remove a script tag
      description: Remove a script tag.
      operationId: deleteAdminScriptTags108074126.json
      x-api-path-slug: adminscript-tags108074126-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Script
      - Tag