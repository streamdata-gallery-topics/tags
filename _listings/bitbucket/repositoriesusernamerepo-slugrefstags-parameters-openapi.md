---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Refs Tags
  description: Parameters repositories username repo slug refs tags
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
  /repositories/{username}/{repo_slug}/refs/tags:
    get:
      summary: Get Repositories Username Repo Slug Refs Tags
      description: Get repositories username repo slug refs tags
      operationId: getRepositoriesUsernameRepoSlugRefsTags
      x-api-path-slug: repositoriesusernamerepo-slugrefstags-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
    parameters:
      summary: Parameters Repositories Username Repo Slug Refs Tags
      description: Parameters repositories username repo slug refs tags
      operationId: parametersRepositoriesUsernameRepoSlugRefsTags
      x-api-path-slug: repositoriesusernamerepo-slugrefstags-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Refs
      - Tags
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