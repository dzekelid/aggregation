---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all searching groups
      description: Returns geoaggregations of all searching groups.
      operationId: Group_GeoAggregationByzoom
      x-api-path-slug: apigroupgeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Searching
      - Groups
  /api/property/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all properties
      description: Returns geoaggregations of all properties.
      operationId: Property_GeoAggregationByzoom
      x-api-path-slug: apipropertygeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Properties
---