---
swagger: "2.0"
info:
  title: AWS Machine Learning API Delete Tags
  version: 1.0.0
  description: Deletes the specified tags associated with an ML object.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteTags:
    get:
      summary: ' Delete Tags '
      description: Deletes the specified tags associated with an ML object
      operationId: deleteTags
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the tagged ML object
        type: string
      - in: query
        name: ResourceType
        description: The type of the tagged ML object
        type: string
      - in: query
        name: TagKeys
        description: One or more tags to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - tags
definitions: []
x-collection-name: AWS Machine Learning
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