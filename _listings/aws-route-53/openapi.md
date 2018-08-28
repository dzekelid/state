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
  /2013-04-01/trafficpolicyinstance/Id:
    get:
      summary: Get Traffic Policy Instance
      description: Gets information about a specified traffic policy instance.Send
        a GET request to the /Amazon Route 53 APIversion/trafficpolicyinstance resource.NoteAfter
        you submit a CreateTrafficPolicyInstance or anUpdateTrafficPolicyInstance
        request, there's a brief delay while Amazon Route 53creates the resource record
        sets that are specified in the traffic policy definition. Formore information,
        see the State response element.NoteIn the Amazon Route 53 console, traffic
        policy instances are known as policy records.
      operationId: gettrafficpolicyinstance
      x-api-path-slug: 20130401trafficpolicyinstanceid-get
      parameters:
      - in: path
        name: Id
        description: The ID of the traffic policy instance that you want to get information
          about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
  ? /2013-04-01/trafficpolicyinstances/hostedzone?id=HostedZoneId&amp;maxitems=MaxItems&amp;trafficpolicyinstancename=TrafficPolicyInstanceNameMarker&amp;trafficpolicyinstancetype=TrafficPolicyInstanceTypeMarker
  : get:
      summary: List Traffic Policy Instances By Hosted Zone
      description: 'Gets information about the traffic policy instances that you created
        in a specifiedhosted zone.NoteAfter you submit an UpdateTrafficPolicyInstance
        request, there''s a briefdelay while Amazon Route 53 creates the resource
        record sets that are specified in the traffic policydefinition. For more information,
        see the State response element.Send a GET request to the /Amazon Route 53
        APIversion/trafficpolicyinstance resource and include the ID of the hostedzone.Amazon
        Route 53 returns a maximum of 100 items in each response. If you have a lot
        of trafficpolicy instances, you can use the MaxItems parameter to list them
        in groups of upto 100.The response includes four values that help you navigate
        from one group ofMaxItems traffic policy instances to the next:             IsTruncated               If
        the value of IsTruncated in the response is true, there aremore traffic policy
        instances associated with the current AWS account.If IsTruncated is false,
        this response includes the lasttraffic policy instance that is associated
        with the current account.             MaxItems           The value that you
        specified for the MaxItems parameter in the requestthat produced the current
        response.                  TrafficPolicyInstanceNameMarker and TrafficPolicyInstanceTypeMarker               If
        IsTruncated is true, these two values in the responserepresent the first traffic
        policy instance in the next group of MaxItemstraffic policy instances. To
        list more traffic policy instances, make another call toListTrafficPolicyInstancesByHostedZone,
        and specify these values in thecorresponding request parameters.If IsTruncated
        is false, all three elements are omittedfrom the response.'
      operationId: listtrafficpolicyinstancesbyhostedzone
      x-api-path-slug: 20130401trafficpolicyinstanceshostedzoneidhostedzoneidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
      parameters:
      - in: path
        name: id
        description: The ID of the hosted zone for which you want to list traffic
          policyinstances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
  ? /2013-04-01/trafficpolicyinstances/trafficpolicy&amp;hostedzoneid=HostedZoneIdMarker?id=TrafficPolicyId&amp;maxitems=MaxItems&amp;trafficpolicyinstancename=TrafficPolicyInstanceNameMarker&amp;trafficpolicyinstancetype=TrafficPolicyInstanceTypeMarker&
  : get:
      summary: List Traffic Policy Instances By Policy
      description: 'Gets information about the traffic policy instances that you created
        by using a specifytraffic policy version.NoteAfter you submit a CreateTrafficPolicyInstance
        or anUpdateTrafficPolicyInstance request, there''s a brief delay while Amazon
        Route 53creates the resource record sets that are specified in the traffic
        policy definition. Formore information, see the State response element.Send
        a GET request to the /Route 53 APIversion/trafficpolicyinstance resource and
        include the ID and version ofthe traffic policy.Amazon Route 53 returns a
        maximum of 100 items in each response. If you have a lot of trafficpolicy
        instances, you can use the MaxItems parameter to list them in groups of upto
        100.The response includes five values that help you navigate from one group
        ofMaxItems traffic policy instances to the next:             IsTruncated               If
        the value of IsTruncated in the response is true,there are more traffic policy
        instances associated with the specified trafficpolicy.If IsTruncated is false,
        this response includes the lasttraffic policy instance that is associated
        with the specified traffic policy.             MaxItems               The
        value that you specified for the MaxItems parameter in the requestthat produced
        the current response.                  HostedZoneIdMarker, TrafficPolicyInstanceNameMarker,
        and TrafficPolicyInstanceTypeMarker               If IsTruncated is true,
        these values in the responserepresent the first traffic policy instance in
        the next group of MaxItemstraffic policy instances. To list more traffic policy
        instances, make another call toListTrafficPolicyInstancesByPolicy, and specify
        these values in thecorresponding request parameters.If IsTruncated is false,
        all three elements are omittedfrom the response.'
      operationId: listtrafficpolicyinstancesbypolicy
      x-api-path-slug: 20130401trafficpolicyinstancestrafficpolicyamphostedzoneidhostedzoneidmarkeridtrafficpolicyidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
      parameters:
      - in: query
        name: CapacityId
        description: The ID that identifies the provisioned capacity unit
        type: string
      - in: query
        name: ExpirationDate
        description: The date that the provisioned capacity unit expires, in Coordinated                            Universal
          Time (UTC)
        type: string
      - in: path
        name: hostedzoneid
        description: For the first request to ListTrafficPolicyInstancesByPolicy,
          omit thisvalue
        type: string
      - in: query
        name: StartDate
        description: The date that the provisioned capacity unit was purchased, in
          Coordinated                            Universal Time (UTC)
        type: string
      - in: query
        name: TagKeys
        description: A list of tag keys
        type: string
      - in: query
        name: Tags
        description: The tags attached to the vault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
  ? /2013-04-01/trafficpolicyinstances?hostedzoneid=HostedZoneIdMarker&amp;maxitems=MaxItems&amp;trafficpolicyinstancename=TrafficPolicyInstanceNameMarker&amp;trafficpolicyinstancetype=TrafficPolicyInstanceTypeMarker
  : get:
      summary: List Traffic Policy Instances
      description: 'Gets information about the traffic policy instances that you created
        by using thecurrent AWS account.NoteAfter you submit an UpdateTrafficPolicyInstance
        request, there''s a briefdelay while Amazon Route 53 creates the resource
        record sets that are specified in the traffic policydefinition. For more information,
        see the State response element.Send a GET request to the /Amazon Route 53
        APIversion/trafficpolicyinstance resource.Amazon Route 53 returns a maximum
        of 100 items in each response. If you have a lot of trafficpolicy instances,
        you can use the MaxItems parameter to list them in groups of upto 100.The
        response includes five values that help you navigate from one group ofMaxItems
        traffic policy instances to the next:             IsTruncated           If
        the value of IsTruncated in the response is true,there are more traffic policy
        instances associated with the current AWSaccount.If IsTruncated is false,
        this response includes the lasttraffic policy instance that is associated
        with the current account.             MaxItems           The value that you
        specified for the MaxItems parameter in the requestthat produced the current
        response.                  HostedZoneIdMarker, TrafficPolicyInstanceNameMarker,
        and TrafficPolicyInstanceTypeMarker               If IsTruncated is true,
        these three values in theresponse represent the first traffic policy instance
        in the next group ofMaxItems traffic policy instances. To list more traffic
        policy instances,make another call to ListTrafficPolicyInstances, and specify
        these values inthe corresponding request parameters.If IsTruncated is false,
        all three elements are omittedfrom the response.'
      operationId: listtrafficpolicyinstances
      x-api-path-slug: 20130401trafficpolicyinstanceshostedzoneidhostedzoneidmarkerampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
      parameters:
      - in: path
        name: hostedzoneid
        description: For the first request to ListTrafficPolicyInstances, omit thisvalue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies