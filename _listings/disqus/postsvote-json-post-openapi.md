---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Posts Vote
  description: Posts Vote
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/vote.json:
    post:
      summary: Posts Vote
      description: Posts Vote
      operationId: posts-vote
      x-api-path-slug: postsvote-json-post
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID
        type: string
      - in: query
        name: vote
        description: 'Choices: -1, 0, 1'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Posts
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