---
name: Google Fit
x-slug: google-fit
description: Google Fit is an open ecosystem that allows developers to upload fitness
  data to a central repository where users can access their data from different devices
  and apps in one location. Fitness apps can store data from any wearable or sensor.
  Fitness apps can access data created by any app. Users fitness data is persisted
  when they upgrade their fitness devices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-fit.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Aggregation
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-fit/apis.md
specificationVersion: "0.14"
apis:
- name: Fitness - Get Aggregate Data
  x-api-slug: useriddatasetaggregate-post
  description: Aggregates data of a certain type or stream into buckets divided by
    a given type of boundary. Multiple data sets of multiple types and from multiple
    sources can be aggreated into exactly one bucket type per request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-fit.jpg
  humanURL: https://developers.google.com/fit/overview
  baseURL: ://www.googleapis.com//fitness/v1/users
  tags: Fitness, Wearables, Google APIs, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-fit/useriddatasetaggregate-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.drive.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.fit.stack.network
- type: x-authentication
  url: https://developers.google.com/fit/android/get-api-key
- type: x-getting-started
  url: https://developers.google.com/fit/rest/v1/get-started
- type: x-website
  url: https://developers.google.com/fit/overview
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---