---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 1
info:
  title: OpenDataSoft
  description: opendatasoft-is-a-cloudbased-turnkey-platform-for-data-publishing-and-api-management--its-interface-is-intuitively-designed-to-empower-anyone-regardless-of-technical-skills-to-upload-easytounderstand-open-data-or-to-even-share-data-within-an-admi---
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
---