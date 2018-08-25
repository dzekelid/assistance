---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Gets details of cases
  description: Gets details of cases
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /assistance/version:
    get:
      summary: Provide basic details about the current deployed version of the assistance
        API
      description: Provide basic details about the current deployed version of the
        assistance API
      operationId: getAssistanceVersion
      x-api-path-slug: assistanceversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - assistance
      - API
  /assistance/v1/home/cases:
    get:
      summary: Gets details of cases
      description: Gets details of cases
      operationId: getAssistanceV1HomeCases
      x-api-path-slug: assistancev1homecases-get
      parameters:
      - in: query
        name: declaration_id
        description: ID of the declaration which has trigger the cases
      - in: query
        name: lastname
        description: Lastname of the person associated to the case
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - detailAssistance
      - of
      - cases
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