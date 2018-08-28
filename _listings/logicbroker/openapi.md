swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Product/{partnerId}/{feedId}/Items/{productId}:
    delete:
      summary: Remove product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_RemoveFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-delete
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      - in: path
        name: productId
        description: Product identifier within the feed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Product
      - Feed
      - Item