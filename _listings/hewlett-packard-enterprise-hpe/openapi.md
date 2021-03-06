swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags:
    get:
      summary: Get Tags
      description: Lists tags.
      operationId: ListTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include each tags related
          `tag-key`'
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Post Tags
      description: Create a tag. It requires the **analyst** global role.
      operationId: CreateTag
      x-api-path-slug: tags-post
      parameters:
      - in: body
        name: tag
        description: New tag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{id}:
    delete:
      summary: Delete Tags
      description: Delete a tag. It requires the **analyst** global role.
      operationId: DeleteTag
      x-api-path-slug: tagsid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag to delete
      responses:
        200:
          description: OK
      tags:
      - Tags
    get:
      summary: Get Tags
      description: Returns a tag based on its id. It requires the **consumer** global
        role.
      operationId: GetTagById
      x-api-path-slug: tagsid-get
      parameters:
      - in: path
        name: id
        description: ID of tag to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include the tags related
          `tag-key`'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tag-keys:
    get:
      summary: Get Tag Keys
      description: Lists tag keys.
      operationId: ListTagKeys
      x-api-path-slug: tagkeys-get
      parameters:
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include each tag-keys
          related `tags`'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
    post:
      summary: Post Tag Keys
      description: Create a tag key. It requires the **analyst** global role.
      operationId: CreateTagKey
      x-api-path-slug: tagkeys-post
      parameters:
      - in: body
        name: name
        description: New tag key
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
  /tag-keys/{id}:
    delete:
      summary: Delete Tag Keys
      description: Delete a tag key and associated tags. It requires the **analyst**
        global role.
      operationId: DeleteTagKey
      x-api-path-slug: tagkeysid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag key to delete
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys
    get:
      summary: Get Tag Keys
      description: Returns a tag key based on its id.
      operationId: GetTagKeyById
      x-api-path-slug: tagkeysid-get
      parameters:
      - in: path
        name: id
        description: ID of tag key to fetch
      - in: query
        name: view
        description: 'Return related resources:  * `full` - Include the tag-keys related
          `tags`'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Keys