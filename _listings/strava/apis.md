---
name: Strava
x-slug: strava
description: Strava is software as a service used to track cycling, running, and swimming
  activity via GPS.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
x-kinRank: "7"
x-alexaRank: "887"
tags: Activity
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/apis.md
specificationVersion: "0.14"
apis:
- name: Strava API v3 - Create an Activity
  x-api-slug: activities-post
  description: Creates a manual activity for an athlete. Requires write permissions,
    as requested during the authorization process.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activities-post-openapi.md
- name: Strava API v3 - Get Activity
  x-api-slug: activitiesid-get
  description: Returns the given activity that is owned by the authenticated athlete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesid-get-openapi.md
- name: Strava API v3 - Update Activity
  x-api-slug: activitiesid-put
  description: Updates the given activity that is owned by the authenticated athlete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesid-put-openapi.md
- name: Strava API v3 - List Activity Laps
  x-api-slug: activitiesidlaps-get
  description: Returns the laps of an activity identified by an identifier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesidlaps-get-openapi.md
- name: Strava API v3 - Get Activity Zones
  x-api-slug: activitiesidzones-get
  description: Premium Feature. Returns the zones of a given activity.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesidzones-get-openapi.md
- name: Strava API v3 - List Activity Comments
  x-api-slug: activitiesidcomments-get
  description: Returns the comments on the given activity.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesidcomments-get-openapi.md
- name: Strava API v3 - List Activity Kudoers
  x-api-slug: activitiesidkudos-get
  description: Returns the athletes who kudoed an activity identified by an identifier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesidkudos-get-openapi.md
- name: Strava API v3 - Upload Activity
  x-api-slug: uploads-post
  description: Uploads a new data file to create an activity from.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/uploads-post-openapi.md
- name: Strava API v3 - Get Activity Streams
  x-api-slug: activitiesidstreams-get
  description: Returns the given activity's streams.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28739-strava.jpg
  humanURL: ""
  baseURL: https://www.strava.com//api/v3
  tags: Mobile, Technology, internet, Sports, Athletes, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/activity/master/_listings/strava/activitiesidstreams-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://storecove.api.gallery.streamdata.io
- type: x-api-stack
  url: http://strava.stack.network
- type: x-code
  url: https://developers.strava.com/docs/#client-code
- type: x-crunchbase
  url: https://crunchbase.com/organization/strava
- type: x-documentation
  url: https://developers.strava.com/docs/reference/
- type: x-email
  url: developers@strava.com
- type: x-email
  url: dpo@strava.com
- type: x-email
  url: ip@strava.com
- type: x-github
  url: https://github.com/strava
- type: x-openapi
  url: https://developers.strava.com/swagger/swagger.json
- type: x-twitter
  url: https://twitter.com/Strava
- type: x-developer
  url: https://developers.strava.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---