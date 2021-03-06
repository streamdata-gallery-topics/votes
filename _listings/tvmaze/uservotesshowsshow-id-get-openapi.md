---
swagger: "2.0"
x-collection-name: TVmaze
x-complete: 0
info:
  title: TVmaze user Get User Votes Shows
  description: Get user votes shows.
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
    get:
      summary: Get User Votes Episodes
      description: Get user votes episodes.
      operationId: getUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
    parameters:
      summary: Parameters User Votes Episodes
      description: Parameters user votes episodes.
      operationId: parametersUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Votes
      - Episodes
    put:
      summary: Put User Votes Episodes
      description: Put user votes episodes.
      operationId: putUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
  /user/votes/shows:
    get:
      summary: Get User Votes Shows
      description: Get user votes shows.
      operationId: getUserVotesShows
      x-api-path-slug: uservotesshows-get
      parameters:
      - in: query
        name: embed
        description: Embed full show info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows
  /user/votes/shows/{show_id}:
    delete:
      summary: Delete User Votes Shows
      description: Delete user votes shows.
      operationId: deleteUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows
    get:
      summary: Get User Votes Shows
      description: Get user votes shows.
      operationId: getUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows
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