---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Returns specific SMART record for
    a patient.
  description: Returns specific smart record for a patient..
  version: 1.0.0
host: rest.ehrscape.com
basePath: /rest/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /smart/records/{ehrId}/{modelName}:
    get:
      summary: Returns SMART records for a patient.
      description: Returns smart records for a patient..
      operationId: getRecords
      x-api-path-slug: smartrecordsehridmodelname-get
      parameters:
      - in: path
        name: ehrId
        description: EHR id
      - in: path
        name: modelName
        description: SMART model name
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Records
      - EhrId
      - ModelName
  /smart/records/{ehrId}/{modelName}/{recordId}:
    get:
      summary: Returns specific SMART record for a patient.
      description: Returns specific smart record for a patient..
      operationId: getRecord
      x-api-path-slug: smartrecordsehridmodelnamerecordid-get
      parameters:
      - in: path
        name: ehrId
        description: EHR id
      - in: path
        name: modelName
        description: SMART model name
      - in: path
        name: recordId
        description: Record id
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Records
      - EhrId
      - ModelName
      - RecordId
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