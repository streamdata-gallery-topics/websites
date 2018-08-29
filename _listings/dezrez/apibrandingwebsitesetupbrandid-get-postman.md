{
  "info": {
    "name": "Dezrez Get files and details that can be used to customize a website",
    "_postman_id": "4115e2df-2c22-4d57-8202-a032408e70f2",
    "description": "Get files and details that can be used to customize a website.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "153444b9-3d4a-4a82-bfdc-7ff1d30166d4",
          "name": "Branding_WebsiteSetupBybrandId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/branding/websitesetup/:brandId"
              ],
              "variable": [
                {
                  "id": "brandId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get files and details that can be used to customize a website."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3a6072b-ee96-4f50-9408-3ffea0ccec17"
            }
          ]
        }
      ]
    }
  ]
}