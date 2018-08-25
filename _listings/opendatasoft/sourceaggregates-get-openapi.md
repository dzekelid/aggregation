---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 0
info:
  title: OpenDataSoft Get Source Aggregates
  description: Compute aggregations from catalog and return a list of each aggregate
    indexed by their names.
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{source}/aggregates:
    get:
      summary: Get Source Aggregates
      description: Compute aggregations from catalog and return a list of each aggregate
        indexed by their names.
      operationId: aggregateDatasets
      x-api-path-slug: sourceaggregates-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Aggregates
  /{source}/datasets/{dataset_id}/aggregates:
    get:
      summary: Get Source Datasets Dataset Aggregates
      description: Compute aggregations from dataset records and return a list of
        each aggregate indexed by their names.
      operationId: aggregateRecords
      x-api-path-slug: sourcedatasetsdataset-idaggregates-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Source
      - Datasets
      - Dataset
      - Id
      - Aggregates
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