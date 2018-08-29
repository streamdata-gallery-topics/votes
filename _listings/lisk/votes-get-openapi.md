---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Requests votes data for an account
  description: |-
    *Attention: At least **one of the filter parameters must be provided.***
    Returns all votes placed by an account.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /votes:
    get:
      summary: Requests votes data for an account
      description: |-
        *Attention: At least **one of the filter parameters must be provided.***
        Returns all votes placed by an account.
      operationId: getVotes
      x-api-path-slug: votes-get
      parameters:
      - in: query
        name: address
        description: Address of an account
      - in: query
        name: limit
        description: Limit applied to results
      - in: query
        name: offset
        description: Offset value for results
      - in: query
        name: publicKey
        description: Public key to query
      - in: query
        name: secondPublicKey
        description: Second public key to query
      - in: query
        name: sort
        description: Fields to sort results by
      - in: query
        name: username
        description: Delegate username to query
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Votes
      - Dataan
      - Account
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