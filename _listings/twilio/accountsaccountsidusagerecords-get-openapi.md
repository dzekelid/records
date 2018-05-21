---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Account Usage Record
  description: Returns UsageRecords for all usage categories. The list includes pagingninformation.nBy
    default, the UsageRecords resource will return one UsageRecord forneach Category,
    representing all usage accrued all-time for the account.nYou can filter the usage
    Category or change the date-range over which usagenis counted using optional GET
    query parameters.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Usage/Records/{Subresource}:
    get:
      summary: Get Account Usage Record Sub Resource
      description: Returns UsageRecords for all usage categories for a specified period.n
      operationId: returns-usagerecords-for-all-usage-categories-for-a-specified-period
      x-api-path-slug: accountsaccountsidusagerecordssubresource-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: Subresource
        description: '|Subresource|Description|n|---|---|n|Daily|Return multiple UsageRecords
          for each usage category, each representing usage over a daily time-interval'
      responses:
        200:
          description: OK
      tags:
      - Usage Records
  /Accounts/{AccountSid}/Usage/Records:
    get:
      summary: Get Account Usage Record
      description: Returns UsageRecords for all usage categories. The list includes
        pagingninformation.nBy default, the UsageRecords resource will return one
        UsageRecord forneach Category, representing all usage accrued all-time for
        the account.nYou can filter the usage Category or change the date-range over
        which usagenis counted using optional GET query parameters.n
      operationId: returns-usagerecords-for-all-usage-categories-the-list-includes-paginginformationby-default-the-usag
      x-api-path-slug: accountsaccountsidusagerecords-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Usage Records
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: "200"
  last_run: ~
  days_run: ~
  minute_run: ~
---