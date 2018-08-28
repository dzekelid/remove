---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Delete Alerts Alert
  description: |-
    ### Delete an Alert

    Removes an alert with the ```alert_id``` from the system.
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