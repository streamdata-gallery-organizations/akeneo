---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API asset (2.1 only)
  description: Asset (2.1 only).
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/assets/paint:
    get:
      summary: asset (2.1 only)
      description: Assuming that the given code is the code of an existing asset
      operationId: RestV1AssetsPaintGet
      x-api-path-slug: restv1assetspaint-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - (2
      - "1"
      - Only)
    patch:
      summary: asset (2.1 only)
      description: Asset (2.1 only).
      operationId: RestV1AssetsPaintPatch
      x-api-path-slug: restv1assetspaint-patch
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
      - Asset
      - (2
      - "1"
      - Only)
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