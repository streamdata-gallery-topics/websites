swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branding/websitesetup/{brandId}:
    get:
      summary: Get files and details that can be used to customize a website
      description: Get files and details that can be used to customize a website.
      operationId: Branding_WebsiteSetupBybrandId
      x-api-path-slug: apibrandingwebsitesetupbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Files
      - Details
      - That
      - Can
      - Be
      - Used
      - To
      - Customize
      - Website