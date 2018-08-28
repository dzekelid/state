---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Describe Instance Patch States For Patch Group
  version: 1.0.0
  description: Retrieves the high-level patch state for the instances in the specified
    patch group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribePatchGroupState:
    get:
      summary: Describe Patch Group State
      description: Returns high-level aggregated patch compliance state for a patch
        group.
      operationId: describePatchGroupState
      x-api-path-slug: actiondescribepatchgroupstate-get
      parameters:
      - in: query
        name: PatchGroup
        description: The name of the patch group whose patch snapshot should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - State
  /?Action=DescribeInstancePatchStates:
    get:
      summary: Describe Instance Patch States
      description: Retrieves the high-level patch state of one or more instances.
      operationId: describeInstancePatchStates
      x-api-path-slug: actiondescribeinstancepatchstates-get
      parameters:
      - in: query
        name: InstanceIds
        description: The ID of the instance whose patch state information should be
          retrieved
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of instances to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - States
  /?Action=DescribeInstancePatchStatesForPatchGroup:
    get:
      summary: Describe Instance Patch States For Patch Group
      description: Retrieves the high-level patch state for the instances in the specified
        patch group.
      operationId: describeInstancePatchStatesForPatchGroup
      x-api-path-slug: actiondescribeinstancepatchstatesforpatchgroup-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group for which the patch state information
          should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - StatesGroup
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