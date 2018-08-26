---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 1
info:
  title: RIPA Node Documentation
  description: this-is-a-documentation-for-ripanodehttpsgithub-comripaexripanode-built-with-swagger-ui-to-make-testing-a-breeze--if-you-find-any-issues-come-over-to-ripaexripanodetestapihttpsgithub-comripaexripanodetestapi-to-open-an-issue-or-even-better-send-a-pr-that-fixes-the-issue-the-community-ssl-public-api-used-as-test-host-is-provided-from-ripaex-iohttpswww-ripaex-io-
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
---