---
swagger: "2.0"
x-collection-name: Vestorly
x-complete: 0
info:
  title: Vestorly Get Groups
  description: Returns all groups
  termsOfService: http://www.vestorly.com/terms/
  contact:
    name: Vestorly Team
  version: 1.0.0
host: staging.vestorly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /advisors/{id}:
    get:
      summary: Get Advisors
      description: Returns a single advisor given their ID
      operationId: findAdvisorByID
      x-api-path-slug: advisorsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Advisor Id to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Advisors
  /articles:
    get:
      summary: Get Articles
      description: Returns all articles
      operationId: findArticles
      x-api-path-slug: articles-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: limit
        description: Limit on the number of articles to return
      - in: query
        name: sort_by
        description: Field on model to sort by
      - in: query
        name: sort_direction
        description: Direction of sort (used with sort_by parameter)
      - in: query
        name: text_query
        description: Search query parameter
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Articles
  /articles/{id}:
    get:
      summary: Get Articles
      description: Returns a single article
      operationId: findArticleByID
      x-api-path-slug: articlesid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Article Id to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Articles
  /events:
    get:
      summary: Get Events
      description: Returns all events
      operationId: findEvents
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: Post Events
      description: Creates a new event in the system
      operationId: createEvent
      x-api-path-slug: events-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: event
        description: Event
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Returns a single event if the user has access
      operationId: findEventByID
      x-api-path-slug: eventsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of event to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Events
  /groups:
    get:
      summary: Get Groups
      description: Returns all groups
      operationId: findGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
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