---
swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeRecord:
    get:
      summary: Describe Record
      description: Retrieves a paginated list of the full details of a specific request.
      operationId: describeRecord
      x-api-path-slug: actiondescriberecord-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The record identifier of the ProvisionedProduct object for which
          to retrieve output         information
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
---