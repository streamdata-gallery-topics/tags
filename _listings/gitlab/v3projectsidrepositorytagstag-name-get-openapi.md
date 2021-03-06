---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Repository Tags Tag Name
  version: 1.0.0
  description: Get projects repository tags tag name.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/repository/tags:
    get:
      summary: Get Projects Repository Tags
      description: Get a project repository tags
      operationId: getV3ProjectsIdRepositoryTags
      x-api-path-slug: v3projectsidrepositorytags-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
    post:
      summary: Post Projects Repository Tags
      description: Post projects repository tags.
      operationId: postV3ProjectsIdRepositoryTags
      x-api-path-slug: v3projectsidrepositorytags-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: message
        description: Specifying a message creates an annotated tag
      - in: formData
        name: ref
        description: The commit sha or branch name
      - in: formData
        name: release_description
        description: Specifying release notes stored in the GitLab database
      - in: formData
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
  /v3/projects/{id}/repository/tags/{tag_name}:
    get:
      summary: Get Projects Repository Tags Tag Name
      description: Get projects repository tags tag name.
      operationId: getV3ProjectsIdRepositoryTagsTagName
      x-api-path-slug: v3projectsidrepositorytagstag-name-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
    delete:
      summary: Delete Projects Repository Tags Tag Name
      description: Delete projects repository tags tag name.
      operationId: deleteV3ProjectsIdRepositoryTagsTagName
      x-api-path-slug: v3projectsidrepositorytagstag-name-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
  /v3/projects/{id}/repository/tags/{tag_name}/release:
    post:
      summary: Post Projects Repository Tags Tag Name Release
      description: Post projects repository tags tag name release.
      operationId: postV3ProjectsIdRepositoryTagsTagNameRelease
      x-api-path-slug: v3projectsidrepositorytagstag-namerelease-post
      parameters:
      - in: formData
        name: description
        description: Release notes with markdown support
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
      - Release
    put:
      summary: Put Projects Repository Tags Tag Name Release
      description: Put projects repository tags tag name release.
      operationId: putV3ProjectsIdRepositoryTagsTagNameRelease
      x-api-path-slug: v3projectsidrepositorytagstag-namerelease-put
      parameters:
      - in: formData
        name: description
        description: Release notes with markdown support
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
      - Release
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