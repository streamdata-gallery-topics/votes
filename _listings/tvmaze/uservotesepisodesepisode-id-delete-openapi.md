---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 0
info:
  title: TVmaze user Delete User Votes Episodes
  description: Delete user votes episodes.
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/votes/episodes:
    get:
      summary: Get User Votes Episodes
      description: Get user votes episodes.
      operationId: getUserVotesEpisodes
      x-api-path-slug: uservotesepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
  /user/votes/episodes/{episode_id}:
    delete:
      summary: Delete User Votes Episodes
      description: Delete user votes episodes.
      operationId: deleteUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
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