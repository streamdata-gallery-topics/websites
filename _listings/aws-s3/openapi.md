swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?website:
    delete:
      summary: DELETE Bucket website
      description: This operation removes the website configuration for a bucket
      operationId: delete-bucket-website
      x-api-path-slug: website-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Website
    get:
      summary: GET Bucket website
      description: This implementation of the GET operation returns the website configurationassociated
        with a bucket
      operationId: get-bucket-website
      x-api-path-slug: website-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Website
    put:
      summary: PUT Bucket website
      description: Sets the configuration of the website that is specified in thewebsite
        subresource
      operationId: put-bucket-website
      x-api-path-slug: website-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Website