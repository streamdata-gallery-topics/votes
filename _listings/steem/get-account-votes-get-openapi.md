---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_account_votes
  description: get_account_votes
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_active_votes:
    get:
      summary: get_active_votes
      description: get_active_votes
      operationId: get-active-votes
      x-api-path-slug: get-active-votes-get
      parameters:
      - in: query
        name: author
        description: account name
      - in: query
        name: permlink
        description: permlink of post
      responses:
        200:
          description: OK
      tags:
      - Get
      - Active
      - Votes
  /get_account_votes:
    get:
      summary: get_account_votes
      description: get_account_votes
      operationId: get-account-votes
      x-api-path-slug: get-account-votes-get
      parameters:
      - in: query
        name: voter
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
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