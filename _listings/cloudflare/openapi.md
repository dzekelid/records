---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 1
info:
  title: CloudFlare
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /zones/:zone_identifier/dns_records:
    get:
      summary: List, search, sort, and filter a zones&#39; DNS records
      description: List, search, sort, and filter a zones&#39; DNS records
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-records-get
      parameters:
      - in: query
        name: content
        description: DNS record contenttttttttttttttt127
      - in: query
        name: direction
        description: Direction to order domainsttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: name
        description: DNS record namettttttttttttttexample
      - in: query
        name: order
        description: Field to order records bytttttttttttttttype
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of DNS records per pagetttttttttttttt20
      - in: query
        name: type
        description: DNS record typettttttttttttttA
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Records
    post:
      summary: Create a new DNS record for a zone
      description: Create a new DNS record for a zone
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-records-post
      parameters:
      - in: query
        name: content
        description: DNS record contenttttttttttttttt127
      - in: query
        name: name
        description: DNS record namettttttttttttttexample
      - in: query
        name: type
        description: DNS record typettttttttttttttA
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Records
  /zones/:zone_identifier/dns_records/:identifier:
    delete:
      summary: 'Delete DNS record permission needed: #dns_records:edit'
      description: 'Delete DNS record permission needed: #dns_records:editntt'
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-recordsidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Records
    get:
      summary: 'DNS record details permission needed: #dns_records:read'
      description: 'DNS record details permission needed: #dns_records:readntt'
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-recordsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Records
    put:
      summary: 'Update DNS record permission needed: #dns_records:edit'
      description: 'Update DNS record permission needed: #dns_records:editntt'
      operationId: cloudflare-dns-records-for-a-zone-api
      x-api-path-slug: zoneszone-identifierdns-recordsidentifier-put
      responses:
        200:
          description: OK
      tags:
      - Records
---