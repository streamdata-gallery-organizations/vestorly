{
  "info": {
    "name": "Vestorly Get Advisors",
    "_postman_id": "d2da9606-343f-455e-a544-a03b9590160b",
    "description": "Returns a single advisor given their ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Advisors",
      "item": [
        {
          "id": "0004dc54-8dda-4f08-89bd-1db05a6e9349",
          "name": "findAdvisorByID",
          "request": {
            "url": {
              "protocol": "http",
              "host": "staging.vestorly.com",
              "path": [
                "api",
                "v2",
                "advisors/:id"
              ],
              "query": [
                {
                  "key": "access_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vestorly-auth",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vestorly_auth",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single advisor given their ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "665a2c8f-eb41-4e64-8cdd-1db4b0bd90bf"
            }
          ]
        }
      ]
    }
  ]
}