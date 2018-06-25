---
name: Rackspace
x-slug: rackspace
description: Host on our dedicated or cloud infrastructure or through one of our partners.
  Leverage our expertise to run fast and lean. We offer web, app or email hosting,
  data services and managed security solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
x-kinRank: "9"
x-alexaRank: "4115"
tags: Records
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/apis.md
specificationVersion: "0.14"
apis:
- name: Rackspace List records
  x-api-slug: rackspace
  description: This call lists all records configured for the specified domain.Note
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/records
  tags: Records
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecords-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecords-get-openapi.md
- name: Rackspace Delete records
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, as described in
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/records
  tags: Records
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecords-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecords-delete-openapi.md
- name: Rackspace Update records
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response. Refer to
    Synchronous and asynchronous responses
    for more details and examples of the way that asynchronous responses work.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/records
  tags: Records
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecords-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecords-put-openapi.md
- name: Rackspace Delete record
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, as described in
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/records/{recordId}
  tags: Records
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecordsrecordid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecordsrecordid-delete-openapi.md
- name: Rackspace Update record
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response. Refer to
    Synchronous and asynchronous responses
    for more details and examples of the way that asynchronous responses work.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/records/{recordId}
  tags: Records
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecordsrecordid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecordsrecordid-put-openapi.md
- name: Rackspace Show record details
  x-api-slug: rackspace
  description: 'This call lists details for a specified record in the specified domain.This
    table shows the possible response codes for this operation:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/records/{recordId}
  tags: Records
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecordsrecordid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/v1-0accountdomainsdomainidrecordsrecordid-get-openapi.md
- name: Rackspace
  x-api-slug: rackspace
  description: Host on our dedicated or cloud infrastructure or through one of our
    partners. Leverage our expertise to run fast and lean. We offer web, app or email
    hosting, data services and managed security solutions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: https:///
  tags: Records
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/rackspace/openapi.md
x-common:
- type: x-base
  url: https://dfw.servers.api.rackspacecloud.com/
- type: x-blog
  url: http://www.rackspace.com/blog/
- type: x-blog-rss
  url: http://www.rackspace.com/blog/feed/rss/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/rackspace
- type: x-crunchbase
  url: https://crunchbase.com/organization/rackspace
- type: x-developer
  url: http://docs.rackspace.com/
- type: x-email
  url: abuse@rackspace.com
- type: x-email
  url: abuse@rackspace.co.uk
- type: x-email
  url: legalnotice@rackspace.com
- type: x-email
  url: rackspacepartners@rackspace.com
- type: x-email
  url: channel@rackspace.co.uk
- type: x-email
  url: asia.partner@rackspace.com
- type: x-email
  url: anz.partner@rackspace.com
- type: x-email
  url: publicrelations@rackspace.com
- type: x-email
  url: michael.house@rackspace.co.uk
- type: x-email
  url: daniela.jimenezparke@rackspace.com
- type: x-github
  url: https://github.com/rackspace
- type: x-pricing
  url: https://www.rackspace.com/calculator
- type: x-twitter
  url: https://twitter.com/rackspace
- type: x-website
  url: http://www.rackspace.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---