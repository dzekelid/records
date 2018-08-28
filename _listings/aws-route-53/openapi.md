swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 1
info:
  title: AWS Route 53 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone:
    post:
      summary: Create Hosted Zone
      description: Creates a new public hosted zone, used to specify how the Domain
        Name System (DNS)routes traffic on the Internet for a domain, such as example.com,
        and its subdomains. ImportantPublic hosted zones can't be converted to a private
        hosted zone or vice versa.Instead, create a new hosted zone with the same
        name and create new resource recordsets.Send a POST request to the /2013-04-01/hostedzone
        resource. The request body must include a documentwith a CreateHostedZoneRequest
        element. The response returns theCreateHostedZoneResponse element containing
        metadata about the hostedzone.Fore more information about charges for hosted
        zones, see Amazon Route 53 Pricing.Note the following:You can't create a hosted
        zone for a top-level domain (TLD).Amazon Route 53 automatically creates a
        default SOA record and four NS records for the zone.For more information about
        SOA and NS records, see NS and SOA Records that Amazon Route 53 Creates for
        a Hosted Zone in the Amazon Route 53 Developer Guide.If your domain is registered
        with a registrar other than Amazon Route 53, you must update thename servers
        with your registrar to make Amazon Route 53 your DNS service. For more information,
        seeConfiguring Amazon Route 53 as your DNSService in the Amazon Route 53 Developer's
        Guide.After creating a zone, its initial status is PENDING. This means that
        itis not yet available on all DNS servers. The status of the zone changes
        to INSYNCwhen the NS and SOA records are available on all Amazon Route 53
        DNS servers. When trying to create a hosted zone using a reusable delegation
        set, specify anoptional DelegationSetId, and Amazon Route 53 would assign
        those 4 NS records for the zone, instead ofallotting a new one.
      operationId: createhostedzone
      x-api-path-slug: 20130401hostedzone-post
      parameters:
      - in: body
        name: CallerReference
        description: A unique string that identifies the request and that allows failedCreateHostedZone
          requests to be retried without the risk of executing theoperation twice
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: CreateHostedZoneRequest
        description: Root level tag for the CreateHostedZoneRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Default
        description: None
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: DelegationSetId
        description: If you want to associate a reusable delegation set with this
          hosted zone, the ID thatAmazon Route 53 assigned to the reusable delegation
          set when you created it
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: HostedZoneConfig
        description: (Optional) A complex type that contains an optional comment about
          your hosted zone
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Name
        description: The name of the domain
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: Parent
        description: CreatedHostedZoneRequest
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: VPC
        description: The VPC that you want your hosted zone to be associated with
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
  /2013-04-01/hostedzone/Id/rrset/:
    post:
      summary: Change Resource Record Sets
      description: 'Create, change, update, or delete authoritative DNS information
        on all Amazon Route 53 servers.Send a POST request to:             /2013-04-01/hostedzone/Amazon
        Route 53 hosted ZoneID/rrset resource. The request body must include a document
        with aChangeResourceRecordSetsRequest element. The request body contains a
        list ofchange items, known as a change batch. Change batches are considered
        transactional changes.When using the Amazon Route 53 API to change resource
        record sets, Amazon Route 53 either makes all or none of thechanges in a change
        batch request. This ensures that Amazon Route 53 never partially implements
        theintended changes to the resource record sets in a hosted zone. For example,
        a change batch request that deletes the CNAME record forwww.example.com and
        creates an alias resource record set for www.example.com. Amazon Route 53
        deletesthe first resource record set and creates the second resource record
        set in a singleoperation. If either the DELETE or the CREATE action fails,
        thenboth changes (plus any other changes in the batch) fail, and the original
        CNAMErecord continues to exist.ImportantDue to the nature of transactional
        changes, you can''t delete the same resourcerecord set more than once in a
        single change batch. If you attempt to delete the same changebatch more than
        once, Amazon Route 53 returns an InvalidChangeBatch error.NoteTo create resource
        record sets for complex routing configurations, use either thetraffic flow
        visual editor in the Amazon Route 53 console or the API actions for traffic
        policies andtraffic policy instances. Save the configuration as a traffic
        policy, then associate thetraffic policy with one or more domain names (such
        as example.com) or subdomain names (suchas www.example.com), in the same hosted
        zone or in multiple hosted zones. You can roll backthe updates if the new
        configuration isn''t performing as expected. For more information, seeUsing
        Traffic Flow to Route DNSTraffic in the Amazon Route 53 Developer Guide.Use
        ChangeResourceRecordsSetsRequest to perform the following actions:                  CREATE:
        Creates a resource record set that has the specified values.                  DELETE:
        Deletes an existing resource record set that has the specified values.                  UPSERT:
        If a resource record set does not already exist, AWS createsit. If a resource
        set does exist, Amazon Route 53 updates it with the values in the request.
        The values that you need to include in the request depend on the type of resource
        record set that you''re creating, deleting, or updating:            Basic
        resource record sets (excluding alias, failover, geolocation, latency, and
        weighted resource record sets)                           Name                                 Type                                 TTL                           Failover,
        geolocation, latency, or weighted resource record sets (excluding alias resource
        record sets)                           Name                                 Type                                 TTL                                 SetIdentifier                           Alias
        resource record sets (including failover alias, geolocation alias, latency
        alias, and weighted alias resource record sets)                           Name                                 Type                                 AliasTarget
        (includes DNSName, EvaluateTargetHealth, and HostedZoneId)                  SetIdentifier
        (for failover, geolocation, latency, and weighted resource record sets)When
        you submit a ChangeResourceRecordSets request, Amazon Route 53 propagates
        your changes to all of the Amazon Route 53 authoritative DNS servers. While
        your changes are propagating, GetChange returns a status of PENDING. When
        propagation is complete, GetChange returns a status of INSYNC. Changes generally
        propagate to all Amazon Route 53 name servers in a few minutes. In rare circumstances,
        propagation can take up to 30 minutes. For more information, see GetChange       For
        information about the limits on a ChangeResourceRecordSets request, see Limits
        in the Amazon Route 53 Developer Guide.'
      operationId: changeresourcerecordsets
      x-api-path-slug: 20130401hostedzoneidrrset-post
      parameters:
      - in: body
        name: ChangeBatch
        description: A complex type that contains an optional comment and the Changeselement
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: ChangeResourceRecordSetsRequest
        description: Root level tag for the ChangeResourceRecordSetsRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The ID of the hosted zone that contains the resource record sets
          that you want tochange
        type: string
      responses:
        200:
          description: OK
      tags:
      - Changes