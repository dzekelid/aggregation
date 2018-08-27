---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Retrieve statistics about this datapoint for a timeframe
  description: Retrieve statistics about this datapoint for a timeframe.
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe
      description: Retrieve statistics about this customer for a timeframe.
      operationId: getAggregated
      x-api-path-slug: aggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: onlyFavorites
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
  /aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getAggregatedList
      x-api-path-slug: aggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - List
  /aggregated/summary/conversions:
    get:
      summary: Retrieve statistics about a subset of conversions for a timeframe with
        conversions data
      description: Retrieve statistics about a subset of conversions for a timeframe
        with conversions data.
      operationId: getAggregatedSummaryConversions
      x-api-path-slug: aggregatedsummaryconversions-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Conversions
  /aggregated/summary/datapoints:
    get:
      summary: Retrieve statistics about a subset of datapoints for a timeframe with
        datapoints data
      description: Retrieve statistics about a subset of datapoints for a timeframe
        with datapoints data.
      operationId: getAggregatedSummaryDatapoints
      x-api-path-slug: aggregatedsummarydatapoints-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupId
        description: Filter by this group id
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Datapoints
  /aggregated/summary/groups:
    get:
      summary: Retrieve statistics about a subset of groups for a timeframe with groups
        data
      description: Retrieve statistics about a subset of groups for a timeframe with
        groups data.
      operationId: getAggregatedSummaryGroups
      x-api-path-slug: aggregatedsummarygroups-get
      parameters:
      - in: query
        name: favourite
        description: Is the group marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Groups
  /conversions/aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe related to
        a subset of conversions grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe related
        to a subset of conversions grouped by some temporal entity (day/week/month).
      operationId: getConversionsAggregatedList
      x-api-path-slug: conversionsaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - Aggregated
      - List
  /conversions/{conversionId}/aggregated:
    get:
      summary: Retrieve statistics about this conversion for a timeframe
      description: Retrieve statistics about this conversion for a timeframe.
      operationId: getConversionsConversionAggregated
      x-api-path-slug: conversionsconversionidaggregated-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: tag
        description: Filter by this tag name
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Aggregated
  /conversions/{conversionId}/aggregated/list:
    get:
      summary: Retrieve statistics about this conversion for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this conversion for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getConversionsConversionAggregatedList
      x-api-path-slug: conversionsconversionidaggregatedlist-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Aggregated
      - List
  /datapoints/aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe by groups
      description: Retrieve statistics about this customer for a timeframe by groups.
      operationId: getDatapointsAggregated
      x-api-path-slug: datapointsaggregated-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Aggregated
  /datapoints/aggregated/list:
    get:
      summary: Retrieve statistics about all datapoints of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all datapoints of this customer for a
        timeframe grouped by some temporal entity (day/week/month).
      operationId: getDatapointsAggregatedList
      x-api-path-slug: datapointsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Aggregated
      - List
  /datapoints/{id}/aggregated:
    get:
      summary: Retrieve statistics about this datapoint for a timeframe
      description: Retrieve statistics about this datapoint for a timeframe.
      operationId: getDatapointsAggregated
      x-api-path-slug: datapointsidaggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Aggregated
  /datapoints/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this datapoint for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this datapoint for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getDatapointsAggregatedList
      x-api-path-slug: datapointsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Aggregated
      - List
  /groups/aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe by groups
      description: Retrieve statistics about this customer for a timeframe by groups.
      operationId: getGroupsAggregated
      x-api-path-slug: groupsaggregated-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
  /groups/aggregated/list:
    get:
      summary: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
      - List
  /groups/{id}/aggregated:
    get:
      summary: Retrieve statistics about this group for a timeframe
      description: Retrieve statistics about this group for a timeframe.
      operationId: getGroupsAggregated
      x-api-path-slug: groupsidaggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
  /groups/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this group for a timeframe grouped by some
        temporal entity (day/week/month)
      description: Retrieve statistics about this group for a timeframe grouped by
        some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - List
  /groups/{id}/aggregated/summary:
    get:
      summary: Retrieve statistics about a subset of datapoints for a timeframe with
        datapoints data
      description: Retrieve statistics about a subset of datapoints for a timeframe
        with datapoints data.
      operationId: getGroupsAggregatedSummary
      x-api-path-slug: groupsidaggregatedsummary-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Filter by this group id
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - Summary
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