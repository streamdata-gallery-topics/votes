---
swagger: "2.0"
x-collection-name: Google Civic Information
x-complete: 0
info:
  title: Google Civic Information API Looks Up Voter Information
  description: Looks up information relevant to a voter based on the voter's registered
    address.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /civicinfo/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /voterinfo:
    get:
      summary: Looks Up Voter Information
      description: Looks up information relevant to a voter based on the voter's registered
        address.
      operationId: civicinfo.elections.voterInfoQuery
      x-api-path-slug: voterinfo-get
      parameters:
      - in: query
        name: address
        description: The registered address of the voter to look up
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: electionId
        description: The unique ID of the election to look up
      - in: query
        name: officialOnly
        description: If set to true, only data from official state sources will be
          returned
      - in: query
        name: returnAllAvailableData
        description: If set to true, the query will return the success codeand include
          any partial information when it is unable to determine a matching address
          or unable to determine the election for electionId=0 queries
      responses:
        200:
          description: OK
      tags:
      - Voter Information
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