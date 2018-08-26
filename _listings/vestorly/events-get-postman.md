{
  "info": {
    "name": "Vestorly Get Events",
    "_postman_id": "1472a3d4-b8e2-42bb-b3e6-6dc7b87cb7ec",
    "description": "Returns all events",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Advisors",
      "item": [
        {
          "id": "cf7bfa5e-db63-4bf6-b1ef-00e99ca1eb78",
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
              "id": "cf2cd9bd-8db7-491d-a3b4-50f8c0d2deca"
            }
          ]
        }
      ]
    },
    {
      "name": "Articles",
      "item": [
        {
          "id": "a0ddb3b5-3fb5-4dba-b85a-a9b79f750d35",
          "name": "findArticles",
          "request": {
            "url": "http://staging.vestorly.com/api/v2/articles?access_token=%7B%7D&limit=%7B%7D&sort_by=%7B%7D&sort_direction=%7B%7D&text_query=%7B%7D&vestorly-auth=%7B%7D&vestorly_auth=%7B%7D",
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
            "description": "Returns all articles"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "406b5c11-2736-48fd-a8d1-3c05660ccd30"
            }
          ]
        },
        {
          "id": "fa0fb134-a221-413d-bdbb-35465315678d",
          "name": "findArticleByID",
          "request": {
            "url": {
              "protocol": "http",
              "host": "staging.vestorly.com",
              "path": [
                "api",
                "v2",
                "articles/:id"
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
            "description": "Returns a single article"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d241b5b6-7b5e-4a63-af1a-e1d647547edf"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "21290d81-a331-4385-b68b-a35b2094d779",
          "name": "findEvents",
          "request": {
            "url": "http://staging.vestorly.com/api/v2/events?access_token=%7B%7D&vestorly-auth=%7B%7D&vestorly_auth=%7B%7D",
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
            "description": "Returns all events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f34e5aab-385f-4701-a770-0af70f906740"
            }
          ]
        }
      ]
    }
  ]
}