---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: Ehr Scape Electronic Health Record APIs
  description: a-simple-yet-powerful-services-to-store-retrieve-and-query-health-data
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
---