---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Remove an existing customer
  description: Remove an existing customer.
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