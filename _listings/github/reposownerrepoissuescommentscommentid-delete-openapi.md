---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Delete Repos Owner Repo Issues Comments Comment
  description: Delete a comment.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gists/{id}/comments/{commentId}:
    delete:
      summary: Delete Gists  Comments Comment
      description: Delete a comment.
      operationId: delete-a-comment
      x-api-path-slug: gistsidcommentscommentid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: commentId
        description: Id of comment
      - in: path
        name: id
        description: Id of gist
      responses:
        200:
          description: OK
      tags:
      - Gists
      - ""
      - Comments
      - Comment
    get:
      summary: Get Gists  Comments Comment
      description: Get a single comment.
      operationId: get-a-single-comment
      x-api-path-slug: gistsidcommentscommentid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: commentId
        description: Id of comment
      - in: path
        name: id
        description: Id of gist
      responses:
        200:
          description: OK
      tags:
      - Gists
      - ""
      - Comments
      - Comment
    patch:
      summary: Patch Gists  Comments Comment
      description: Edit a comment.
      operationId: edit-a-comment
      x-api-path-slug: gistsidcommentscommentid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: Id of comment
      - in: path
        name: id
        description: Id of gist
      responses:
        200:
          description: OK
      tags:
      - Gists
      - ""
      - Comments
      - Comment
  /repos/{owner}/{repo}/comments/{commentId}:
    delete:
      summary: Delete Repos Owner Repo Comments Comment
      description: Delete a commit comment
      operationId: delete-a-commit-comment
      x-api-path-slug: reposownerrepocommentscommentid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: commentId
        description: Id of comment
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Comments
      - Comment
    get:
      summary: Get Repos Owner Repo Comments Comment
      description: Get a single commit comment.
      operationId: get-a-single-commit-comment
      x-api-path-slug: reposownerrepocommentscommentid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: commentId
        description: Id of comment
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Comments
      - Comment
    patch:
      summary: Patch Repos Owner Repo Comments Comment
      description: Update a commit comment.
      operationId: update-a-commit-comment
      x-api-path-slug: reposownerrepocommentscommentid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: Id of comment
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Comments
      - Comment
  /repos/{owner}/{repo}/issues/comments/{commentId}:
    delete:
      summary: Delete Repos Owner Repo Issues Comments Comment
      description: Delete a comment.
      operationId: delete-a-comment
      x-api-path-slug: reposownerrepoissuescommentscommentid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: commentId
        description: ID of comment
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Comments
      - Comment
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