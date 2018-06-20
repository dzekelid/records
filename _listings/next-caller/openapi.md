---
swagger: "2.0"
x-collection-name: Next Caller
x-complete: 1
info:
  title: Next Caller
  description: advanced-caller-id--obtain-name-address-and-email-of-your-inbound-callers-
  version: 1.0.0
host: api.sandbox.nextcaller.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/records/:
    parameters:
      summary: Parameters Version Records
      description: Parameters version records.
      operationId: parametersVersionRecords
      x-api-path-slug: versionrecords-parameters
      responses:
        200:
          description: OK
      tags:
      - Version
      - Records
    get:
      summary: Get Version Records
      description: Returns Nextcaller member detailed info.
      operationId: getVersionRecords
      x-api-path-slug: versionrecords-get
      parameters:
      - in: query
        name: format
        description: 'Specifies a format of response: JSON or XML'
      - in: query
        name: phone
        description: Specifies the callers phone number
      - in: path
        name: version
        description: Specifies a api version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Records
---