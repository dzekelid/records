swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/group/recordcontact:
    post:
      summary: Records an event on the group representing a neg being in contact
      description: Records an event on the group representing a neg being in contact.
      operationId: Group_RecordContactByrecordGroupContactDataContract
      x-api-path-slug: apigrouprecordcontact-post
      parameters:
      - in: body
        name: recordGroupContactDataContract
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
      - Group
      - Representing
      - Neg
      - Being
      - In
      - Contact
  /api/receipt/fundsshortfall:
    post:
      summary: Records funds from office account into client account and then to client
        if necessary.
      description: Records funds from office account into client account and then
        to client if necessary..
      operationId: Receipt_ReceiptFundsShortfallBydataContract
      x-api-path-slug: apireceiptfundsshortfall-post
      parameters:
      - in: body
        name: dataContract
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
      - Funds
      - From
      - Office
      - Account
      - Into
      - Client
      - Account
      - Then
      - To
      - Client
      - If
      - Necessary