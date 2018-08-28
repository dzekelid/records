swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 1
info:
  title: SalesLoft
  description: salesloft-helps-transform-sales-teams-into-modern-sales-organizations---converting-more-target-accounts-into-customer-accounts
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/call_data_records.json:
    get:
      summary: List call data records
      description: |-
        Fetches multiple call data records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Call data records are records of all inbound and outbound calls through SalesLoft. A call data record may
        be associated with a call, but does not have to be.
      operationId: v2.call_data_records.json.get
      x-api-path-slug: v2call-data-records-json-get
      parameters:
      - in: query
        name: has_call
        description: Return only call data records which have or do not have a call
          logged for them
      - in: query
        name: ids
        description: IDs of call data records to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Call
      - Data
      - Records