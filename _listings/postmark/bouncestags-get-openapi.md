---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Get Bounces Tags
  description: Returns a list of tags used for the current server.
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bounces/tags:
    parameters:
      summary: Parameters Bounces Tags
      description: Parameters bounces tags.
      operationId: parametersBouncesTags
      x-api-path-slug: bouncestags-parameters
      responses:
        200:
          description: OK
      tags:
      - Bounces
      - Tags
    get:
      summary: Get Bounces Tags
      description: Returns a list of tags used for the current server.
      operationId: getBouncesTags
      x-api-path-slug: bouncestags-get
      parameters:
      - in: query
        name: Accept
        description: The accepted type for the response
      - in: query
        name: Content-Type
        description: The content type of the request
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Bounces
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