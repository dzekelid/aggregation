---
name: Google Compute Engine
x-slug: google-compute-engine
description: Google Compute Engine delivers virtual machines running in Googles innovative
  data centers and worldwide fiber network. Compute Engines tooling and workflow support
  enable scaling from single instances to global, load-balanced cloud computing.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Aggregation
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/apis.md
specificationVersion: "0.14"
apis:
- name: Google Compute Engine API Get Addresses
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of addresses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/addresses
  tags: Address,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedaddresses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedaddresses-get-openapi.md
- name: Google Compute Engine API Get Autoscalers
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of autoscalers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/autoscalers
  tags: Autoscaler,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedautoscalers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedautoscalers-get-openapi.md
- name: Google Compute Engine API Get Backend services
  x-api-slug: google-compute-engine-api
  description: Retrieves the list of all BackendService resources, regional and global,
    available to the specified project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/backendServices
  tags: Backend Service,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedbackendservices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedbackendservices-get-openapi.md
- name: Google Compute Engine API Get Disk Type
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of disk types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/diskTypes
  tags: Disk,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregateddisktypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregateddisktypes-get-openapi.md
- name: Google Compute Engine API Get Disks
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of persistent disks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/disks
  tags: Disk,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregateddisks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregateddisks-get-openapi.md
- name: Google Compute Engine API Get Forwarding Rules
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of forwarding rules.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/forwardingRules
  tags: Forwarding Rules,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedforwardingrules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedforwardingrules-get-openapi.md
- name: Google Compute Engine API Get Instance Groups
  x-api-slug: google-compute-engine-api
  description: Retrieves the list of instance groups and sorts them by zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/instanceGroups
  tags: Instance Group,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedinstancegroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedinstancegroups-get-openapi.md
- name: Google Compute Engine API Get Instances
  x-api-slug: google-compute-engine-api
  description: Retrieves aggregated list of instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/instances
  tags: Instance,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedinstances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedinstances-get-openapi.md
- name: Google Compute Engine API Get Machine Types
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of machine types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/machineTypes
  tags: Machine,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedmachinetypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedmachinetypes-get-openapi.md
- name: Google Compute Engine API Get Operations
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of all operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/operations
  tags: Operation,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedoperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedoperations-get-openapi.md
- name: Google Compute Engine API Get Routers
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of routers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/routers
  tags: Router,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedrouters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedrouters-get-openapi.md
- name: Google Compute Engine API Get Subnetworks
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of subnetworks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/subnetworks
  tags: Subnetwork,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedsubnetworks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedsubnetworks-get-openapi.md
- name: Google Compute Engine API Get Target Instances
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of target instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/targetInstances
  tags: Target Instance,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedtargetinstances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedtargetinstances-get-openapi.md
- name: Google Compute Engine API Get Target Pools
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of target pools.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/targetPools
  tags: Target Pools,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedtargetpools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedtargetpools-get-openapi.md
- name: Google Compute Engine API Get Target VPN Gateways
  x-api-slug: google-compute-engine-api
  description: Retrieves an aggregated list of target VPN gateways.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects//{project}/aggregated/targetVpnGateways
  tags: Target VPN Gateway,Aggregation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedtargetvpngateways-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/projectaggregatedtargetvpngateways-get-openapi.md
- name: Google Compute Engine API
  x-api-slug: google-compute-engine-api
  description: Google Compute Engine delivers virtual machines running in Googles
    innovative data centers and worldwide fiber network. Compute Engines tooling and
    workflow support enable scaling from single instances to global, load-balanced
    cloud computing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Aggregation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/aggregation/master/_listings/google-compute-engine/openapi.md
x-common:
- type: x-code
  url: https://cloud.google.com/compute/docs/api/libraries
- type: x-documentation
  url: https://cloud.google.com/compute/docs/reference/latest/
- type: x-guides
  url: https://cloud.google.com/compute/docs/api/how-tos/how-tos
- type: x-rate-limits
  url: https://cloud.google.com/compute/docs/api-rate-limits
- type: x-sla
  url: https://cloud.google.com/compute/sla
- type: x-website
  url: https://cloud.google.com/compute/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---