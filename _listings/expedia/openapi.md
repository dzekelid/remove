swagger: "2.0"
x-collection-name: Expedia
x-complete: 1
info:
  title: Expedia
  description: expedia-mobile-api-documentation--brfont-colorblue-note-in-case-of-authorization-exception-just-a-hrefstaticmobileswaggeruiusersigninusersigninafont
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