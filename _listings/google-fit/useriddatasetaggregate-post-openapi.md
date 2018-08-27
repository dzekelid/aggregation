---
swagger: "2.0"
x-collection-name: Google Fit
x-complete: 0
info:
  title: Google Fit API Get Aggregate Data
  description: Aggregates data of a certain type or stream into buckets divided by
    a given type of boundary. Multiple data sets of multiple types and from multiple
    sources can be aggreated into exactly one bucket type per request.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /fitness/v1/users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{userId}/dataset:aggregate:
    post:
      summary: Get Aggregate Data
      description: Aggregates data of a certain type or stream into buckets divided
        by a given type of boundary. Multiple data sets of multiple types and from
        multiple sources can be aggreated into exactly one bucket type per request.
      operationId: fitness.users.dataset.aggregate
      x-api-path-slug: useriddatasetaggregate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: Aggregate data for the person identified
      responses:
        200:
          description: OK
      tags:
      - Aggregation
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