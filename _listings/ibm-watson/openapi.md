swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 1
info:
  title: IBM Watson Machine Learning API
  description: -authorizationstep-by-step-instruction-how-to-use-watson-machine-learning-servicecan-be-found-herehttpsdatascience-ibm-comdocscontentanalyzedatamloverview-htmlcontextanalytics-ibm-watson-machine-learning-credentialsto-start-working-with-api-one-needs-to-generate-an-access-token-using-the-username-and-passwordavailable-on-the-service-credentials-tab-of-the-ibm-watson-machine-learning-service-instance-or-also-available-in-the-vcap-environment-variable-example-of-the-service-credentialsjson----url-httpsibmwatsonml-mybluemix-net----username-c1ef4b802ee2458eab92e9ca97ec657d----password-030528d45a3e4d4c92585d553513be6f----instance-id-a751c209954edc32b441ad56ce7a9f40example-of-obtaining-access-token-from-token-endpoint-using-http-basic-auth-for-details-please-refer-to-token-section-belowcurl-basic-user-usernamepassword-httpsibmwatsonml-mybluemix-netv3identitytokenthe-obtained-access-token-needs-to-be-prepended-with-bearer-word-and-it-needs-to-be-passed-in-the-authorization-header-for-api-calls-example-of-api-request-with-bearer-access-tokencurl-httpsibmwatsonml-mybluemix-netv3wml-instances00fd89e68cf24712a068ade10277b649published-models-h-authorization-bearer-eyjhbgcioijsuzuxmiisinr5cci6ikpxvcj9-eyj0zw5hbnrjzci6imu4ymqzzgm3lwi5y2utndy1oc1iz----apache-spark-service-credentialsthe-ibm-watson-machine-learning-cooperates-with-the-apache-spark-as-a-service-to-create-batch-stream-deploymentsand-for-learning-configuration-functionality-for-api-methods-requiring-apache-spark-service-instance-a-custom-header-xsparkserviceinstancewith-service-credentials-must-be-specified-the-header-value-is-a-base64-encoded-string-with-the-json-data-containing-service-credentials-and-spark-version-example-of-the-json-data---credentials------tenant-ids068ade10277b6495605b1d10fv12b------tenant-id-full00fd89e68cf24712a068ade10277b649-41f37bf21b954c65a15605b1d10fb12b------cluster-master-urlhttpsspark-bluemix-net------instance-id00fd89e68cf24712a068ade10277b649------tenant-secretc74c37cf482a4da4836ef32ca26ccbb9------planibm-sparkservice-paygopersonal------version2-0
  version: 1.0.0
basePath: v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device/types/{typeId}/devices/{deviceId}/state/{logicalInterfaceId}:
    get:
      summary: Get the state for the device with the specified id
      description: Retrieve the current state of the device with the specified id.
      operationId: retrieve-the-current-state-of-the-device-with-the-specified-id
      x-api-path-slug: devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
      - Devices
      - DeviceId
      - State
      - LogicalInterfaceId
    patch:
      summary: Perform an operation against the device state for a logical interface
      description: |-
        Performs the specified operation against the device state for a logical
        interface. The following values can be specified for the operation
        property:

          - reset-state

        The **reset-state** operation will reset the state of the specified
        device to the default values as defined by the schema for the logical
        interface.
      operationId: performs-the-specified-operation-against-the-device-state-for-a-logicalinterface-the-following-value
      x-api-path-slug: devicetypestypeiddevicesdeviceidstatelogicalinterfaceid-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Operation
        description: The JSON representation of an operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
      - Devices
      - DeviceId
      - State
      - LogicalInterfaceId
  /thing/types/{thingTypeId}/things/{thingId}/state/{logicalInterfaceId}:
    get:
      summary: Get the state for the thing with the specified id
      description: Retrieve the current state of the thing with the specified id.
      operationId: retrieve-the-current-state-of-the-thing-with-the-specified-id
      x-api-path-slug: thingtypesthingtypeidthingsthingidstatelogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Thing
      - Types
      - ThingTypeId
      - Things
      - ThingId
      - State
      - LogicalInterfaceId
    patch:
      summary: Perform an operation against the thing state for a logical interface
      description: |-
        Performs the specified operation against the thing state for a logical
        interface. The following values can be specified for the operation
        property:

          - reset-state

        The **reset-state** operation will reset the state of the specified
        thing instance to the default values as defined by the schema for the
        logical interface.
      operationId: performs-the-specified-operation-against-the-thing-state-for-a-logicalinterface-the-following-values
      x-api-path-slug: thingtypesthingtypeidthingsthingidstatelogicalinterfaceid-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Operation
        description: The JSON representation of an operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Thing
      - Types
      - ThingTypeId
      - Things
      - ThingId
      - State
      - LogicalInterfaceId
host: ibm-watson-ml.mybluemix.net