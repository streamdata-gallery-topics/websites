---
swagger: "2.0"
x-collection-name: Google Site Verification
x-complete: 0
info:
  title: Google Site Verification API Get Verified Websites
  description: Get the list of your verified websites and domains.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /siteVerification/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webResource:
    get:
      summary: Get Verified Websites
      description: Get the list of your verified websites and domains.
      operationId: siteVerification.webResource.list
      x-api-path-slug: webresource-get
      responses:
        200:
          description: OK
      tags:
      - Website
    post:
      summary: Verify Website
      description: Attempt verification of a website or domain.
      operationId: siteVerification.webResource.insert
      x-api-path-slug: webresource-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: verificationMethod
        description: The method to use for verifying a site or domain
      responses:
        200:
          description: OK
      tags:
      - Website
  /webResource/{id}:
    delete:
      summary: Relinquish Ownership Of Website
      description: Relinquish ownership of a website or domain.
      operationId: siteVerification.webResource.delete
      x-api-path-slug: webresourceid-delete
      parameters:
      - in: path
        name: id
        description: The id of a verified site or domain
      responses:
        200:
          description: OK
      tags:
      - Website
    get:
      summary: Get Current Data for Website
      description: Get the most current data for a website or domain.
      operationId: siteVerification.webResource.get
      x-api-path-slug: webresourceid-get
      parameters:
      - in: path
        name: id
        description: The id of a verified site or domain
      responses:
        200:
          description: OK
      tags:
      - Website
    patch:
      summary: Update List of Owners for Website
      description: Modify the list of owners for your website or domain. This method
        supports patch semantics.
      operationId: siteVerification.webResource.patch
      x-api-path-slug: webresourceid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of a verified site or domain
      responses:
        200:
          description: OK
      tags:
      - Website
    put:
      summary: Update List of Owners for Website
      description: Modify the list of owners for your website or domain.
      operationId: siteVerification.webResource.update
      x-api-path-slug: webresourceid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of a verified site or domain
      responses:
        200:
          description: OK
      tags:
      - Website
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