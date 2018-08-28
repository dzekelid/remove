swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 1
info:
  title: ClimaCell API
  description: the-climacell-rest-api-provides-access-to-high-resolution-weather-data-for-locations-across-the-u-s--with-global-data-coming-soon--it-uses-https-and-requires-an-access-token-key--the-api-requests-carry-query-parameters-and-the-responses-return-results-in-json-format-
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts/{alert_id}:
    delete:
      summary: Delete Alerts Alert
      description: |-
        ### Delete an Alert

        Removes an alert with the ```alert_id``` from the system.
      operationId: -delete-an-alertremoves-an-alert-with-the-alert-id-from-the-system
      x-api-path-slug: alertsalert-id-delete
      parameters:
      - in: path
        name: alert_id
        description: UUID of the Alert
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
      - Alert