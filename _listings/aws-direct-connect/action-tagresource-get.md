---
swagger: "2.0"
info:
  title: AWS Direct Connect API Tag Resource
  version: 1.0.0
  description: Adds the specified tags to the specified Direct Connect resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TagResource:
    get:
      summary: ' Tag Resource '
      description: Adds the specified tags to the specified Direct Connect resource
      operationId: tagResource
      parameters:
      - in: query
        name: resourceArn
        description: The Amazon Resource Name (ARN) of the Direct Connect resource
        type: string
      - in: query
        name: tags
        description: The list of tags to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - resource tags
definitions: []
x-collection-name: AWS Direct Connect
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