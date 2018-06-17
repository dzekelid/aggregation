---
swagger: "2.0"
x-collection-name: Google Fit
x-complete: 1
info:
  title: Fitness
  description: stores-and-accesses-user-data-in-the-fitness-store-from-apps-on-any-platform-
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
---