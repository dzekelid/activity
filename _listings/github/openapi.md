swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/stats/commit_activity:
    get:
      summary: Get Repos Owner Repo Stats Commit Activity
      description: |-
        Get the last year of commit activity data.
        Returns the last year of commit activity grouped by week. The days array
        is a group of commits per day, starting on Sunday.
      operationId: get-the-last-year-of-commit-activity-datareturns-the-last-year-of-commit-activity-grouped-by-week-th
      x-api-path-slug: reposownerrepostatscommit-activity-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Stats
      - Commit
      - Activity