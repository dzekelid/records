---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Records an event on the role representing a neg being in contact with
    a person
  version: 1.0.0
  description: Records an event on the role representing a neg being in contact with
    a person.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/event/recordpropertyownercontact:
    post:
      summary: Records an event on the role representing a neg being in contact for
        a property they own
      description: Records an event on the role representing a neg being in contact
        for a property they own.
      operationId: Event_RecordPropertyOwnerContactByrecordPropertyOwnerContactDataContract
      x-api-path-slug: apieventrecordpropertyownercontact-post
      parameters:
      - in: body
        name: recordPropertyOwnerContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contacta
      - Property
      - They
      - Own
  /api/event/recordownercontact:
    post:
      summary: Records an event on the role representing a neg being in contact for
        an owner
      description: Records an event on the role representing a neg being in contact
        for an owner.
      operationId: Event_RecordOwnerContactByrecordOwnerContactDataContract
      x-api-path-slug: apieventrecordownercontact-post
      parameters:
      - in: body
        name: recordOwnerContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contactan
      - Owner
  /api/event/recordenquiry:
    post:
      summary: Records an event on the role representing a neg being in contact with
        a person
      description: Records an event on the role representing a neg being in contact
        with a person.
      operationId: Event_RecordEnquiryByrecordEnquiryDataContract
      x-api-path-slug: apieventrecordenquiry-post
      parameters:
      - in: body
        name: recordEnquiryDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contact
      - Person
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