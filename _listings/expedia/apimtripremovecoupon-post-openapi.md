---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Remove Coupon
  description: Mobile API Packages Remove Coupon
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/m/trip/remove/coupon:
    post:
      summary: Remove Coupon
      description: Mobile API Packages Remove Coupon
      operationId: packages-remove-coupon
      x-api-path-slug: apimtripremovecoupon-post
      parameters:
      - in: formData
        name: tripId
        description: The tripId we are going to apply the coupon to
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Airports
      - Airplanes
      - Coupons
      - Airlines
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