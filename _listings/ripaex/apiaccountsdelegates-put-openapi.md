---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Accounts Delegates
  description: Vote for a delegate by public key.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/delegates/voters:
    get:
      summary: Delegates Voters
      description: Get a list of voters for a delegate.
      operationId: delegates.getVoters
      x-api-path-slug: apidelegatesvoters-get
      parameters:
      - in: query
        name: publicKey
        description: A valid RIPA Public Key
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Voters
  /api/accounts/delegates:
    put:
      summary: Accounts Delegates
      description: Vote for a delegate by public key.
      operationId: accounts.addDelegates
      x-api-path-slug: apiaccountsdelegates-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Delegates
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