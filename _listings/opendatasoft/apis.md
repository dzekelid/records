---
name: OpenDataSoft
x-slug: opendatasoft
description: OpenDataSoft is a cloud-based turnkey platform for data publishing and
  API management. Its interface is intuitively designed to empower anyone, regardless
  of technical skills, to upload easy-to-understand Open Data, or to even share data
  within an admi...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
x-kinRank: "7"
x-alexaRank: "307560"
tags: Records
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/opendatasoft/apis.md
specificationVersion: "0.14"
apis:
- name: OpenDataSoft Get Source Datasets Dataset Records
  x-api-slug: opendatasoft
  description: Search dataset's records.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2//{source}/datasets/{dataset_id}/records
  tags: Source,Datasets,Dataset,Id,Records
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/opendatasoft/sourcedatasetsdataset-idrecords-get-openapi.md
- name: OpenDataSoft Get Source Datasets Dataset Records Record
  x-api-slug: opendatasoft
  description: Retrieve a single record based on its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2//{source}/datasets/{dataset_id}/records/{record_id}
  tags: Source,Datasets,Dataset,Id,Records,Record,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/opendatasoft/sourcedatasetsdataset-idrecordsrecord-id-get-openapi.md
- name: OpenDataSoft
  x-api-slug: opendatasoft
  description: OpenDataSoft is a cloud-based turnkey platform for data publishing
    and API management. Its interface is intuitively designed to empower anyone, regardless
    of technical skills, to upload easy-to-understand Open Data, or to even share
    data within an admi...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2716-opendatasoft.jpg
  humanURL: http://opendatasoft.com
  baseURL: https://public.opendatasoft.com//api/v2
  tags: Records
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/records/master/_listings/opendatasoft/openapi.md
x-common:
- type: x-blog
  url: http://www.opendatasoft.com/category/news/
- type: x-crunchbase
  url: https://crunchbase.com/organization/opendatasoft
- type: x-crunchbase
  url: http://www.crunchbase.com/company/opendatasoft
- type: x-email
  url: contact@opendatasoft.com
- type: x-email
  url: cil@opendatasoft.com
- type: x-twitter
  url: https://twitter.com/opendatasoft
- type: x-website
  url: http://opendatasoft.com
- type: x-website
  url: https://www.opendatasoft.com
- type: x-website
  url: http://www.opendatasoft.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---