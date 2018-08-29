---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Delete a website
  description: Delete a website with predefined identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /websites:
    get:
      summary: Retrieve a list of websites
      description: Retrieve a list of websites
      operationId: retrieve-a-list-of-websites
      x-api-path-slug: websites-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Websites
    post:
      summary: Create a website
      description: Create a website
      operationId: create-a-website
      x-api-path-slug: websites-post
      parameters:
      - in: body
        name: body
        description: Website resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Website
  /websites/{id}:
    delete:
      summary: Delete a website
      description: Delete a website with predefined identifier string
      operationId: delete-a-website-with-predefined-identifier-string
      x-api-path-slug: websitesid-delete
      responses:
        200:
          description: OK
      tags:
      - Website
    get:
      summary: Retrieve a website
      description: Retrieve a website with specified identifier string
      operationId: retrieve-a-website-with-specified-identifier-string
      x-api-path-slug: websitesid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Website
    put:
      summary: Create or update a website with predefined ID
      description: Create or update a website with predefined identifier string
      operationId: create-or-update-a-website-with-predefined-identifier-string
      x-api-path-slug: websitesid-put
      parameters:
      - in: body
        name: body
        description: Website resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Website
      - Predefined
      - ID
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