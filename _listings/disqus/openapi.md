swagger: "2.0"
x-collection-name: Disqus
x-complete: 1
info:
  title: Disqus
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
  /threads/vote.json:
    post:
      summary: Threads Vote
      description: Threads Vote
      operationId: threads-vote
      x-api-path-slug: threadsvote-json-post
      parameters:
      - in: query
        name: forum
        description: Defaults to null                         Looks up a forum by
          ID (aka short name)
        type: string
      - in: query
        name: thread
        description: Looks up a thread by ID You may pass us the &#39;ident&#39; or
          &#39;link&#39; query types instead of an ID by including &#39;forum&#39;
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
      - Threads
      - Vote