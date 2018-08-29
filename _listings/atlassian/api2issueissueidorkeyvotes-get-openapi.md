---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get votes
  description: Returns voting data for an issue - whether the issue was voted for,
    total number of votes and users who voted for the issue.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/votes:
    get:
      summary: Get votes
      description: Returns voting data for an issue - whether the issue was voted
        for, total number of votes and users who voted for the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getVotes_get
      x-api-path-slug: api2issueissueidorkeyvotes-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve voting information for
      responses:
        200:
          description: OK
      tags:
      - Votes
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