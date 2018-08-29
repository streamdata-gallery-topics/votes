---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Get Repositories Username Repo Slug Issues Issue  Vote
  description: |-
    Check whether the authenticated user has voted for this issue.
    A 204 status code indicates that the user has voted, while a 404
    implies they haven't.
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/issues/{issue_id}/vote:
    delete:
      summary: Delete Repositories Username Repo Slug Issues Issue  Vote
      description: Delete repositories username repo slug issues issue  vote
      operationId: deleteRepositoriesUsernameRepoSlugIssuesIssueVote
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idvote-delete
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Vote
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Vote
      description: |-
        Check whether the authenticated user has voted for this issue.
        A 204 status code indicates that the user has voted, while a 404
        implies they haven't.
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueVote
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idvote-get
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Vote
    parameters:
      summary: Parameters Repositories Username Repo Slug Issues Issue  Vote
      description: Parameters repositories username repo slug issues issue  vote
      operationId: parametersRepositoriesUsernameRepoSlugIssuesIssueVote
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idvote-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Vote
    put:
      summary: Update Repositories Username Repo Slug Issues Issue  Vote
      description: |-
        Vote for this issue.

        To cast your vote, do an empty PUT. The 204 status code indicates that
        the operation was successful.
      operationId: putRepositoriesUsernameRepoSlugIssuesIssueVote
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idvote-put
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
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