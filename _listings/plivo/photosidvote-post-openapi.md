---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Photos Vote
  description: Allows the user to vote for a photo.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/:id/votes:
    get:
      summary: Get Photos Votes
      description: Returns all users that had liked this photo.
      operationId: returns-all-users-that-had-liked-this-photo
      x-api-path-slug: photosidvotes-get
      parameters:
      - in: query
        name: page
        description: Return a specific page in the photo stream
      - in: query
        name: rpp
        description: The number of results to return
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
      - Votes
  /photos/:id/vote:
    post:
      summary: Post Photos Vote
      description: Allows the user to vote for a photo.
      operationId: allows-the-user-to-vote-for-a-photo
      x-api-path-slug: photosidvote-post
      parameters:
      - in: query
        name: id (required)
        description: ID of the photo the vote is cast upon
      - in: query
        name: vote (required)
        description: 'vote, values: 0 for dislike or 1 for like'
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
      - Vote
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