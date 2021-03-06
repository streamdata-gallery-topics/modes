swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/execution/async:
    post:
      summary: Execute the specified orchestration in asynchronous mode.
      description: To successfully execute the orchestration, the OrchestrationExecutionRequest
        must contain valid orchestration id, asset id, asset data field mapping details.
      operationId: runAsync
      x-api-path-slug: apiv2executionasync-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
      - In
      - Asynchronous
      - Mode