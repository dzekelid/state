---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Update the chat:glance state
  description: Authentication required, with scope participate:conversation
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/user/search/query:
    get:
      summary: Find users by query
      description: |-
        Finds users using a structured query and returns user details. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse users and groups_ [global permission](href=). The available queries statements are:

        `is assignee of PROJ` Returns the users that are assignees of at least one issue in project _PROJ_.*   `is assignee of (PROJ-1, PROJ-2)` Returns users that are assignees on the issues _PROJ-1_ or _PROJ-2_.
        *   `is reporter of (PROJ-1, PROJ-2)` Returns users that are reporters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is watcher of (PROJ-1, PROJ-2)` Returns users that are watchers on the issues _PROJ-1_ or _PROJ-2_.
        *   `is voter of (PROJ-1, PROJ-2)` Returns users that are voters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is commenter of (PROJ-1, PROJ-2)` Returns users that have posted a comment on the issues _PROJ-1_ or _PROJ-2_.
        *   `is transitioner of (PROJ-1, PROJ-2)` Returns users that have performed a transition on issues _PROJ-1_ or _PROJ-2_.
        *   `[propertyKey].entity.property.path is "property value"` Returns users with the entity property value.

        The list of issues can be extended as needed, as in _(PROJ-1, PROJ-2, ... PROJ-n)_. Statements can be combined using the `AND` and `OR` operators to form more complex queries, for example:

        `is assignee of PROJ AND [propertyKey].entity.property.path is "property value"`
      operationId: com.atlassian.jira.rest.v2.search.UserSearchResource.findUsersByQuery_get
      x-api-path-slug: api2usersearchquery-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: includeInactive
        description: Include inactive users in the results
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: query
        description: The search query
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - By
      - Query
  /api/2/user/search/query/key:
    get:
      summary: Find user keys by query
      description: |-
        Finds users using a structured query and returns a list of user keys. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse users and groups_ [global permission](href=). The available query statements are:

        *   `is assignee of PROJ` Returns the users that are assignees of at least one issue in project _PROJ_.
        *   `is assignee of (PROJ-1, PROJ-2)` Returns users that are assignees on the issues _PROJ-1_ or _PROJ-2_.
        *   `is reporter of (PROJ-1, PROJ-2)` Returns users that are reporters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is watcher of (PROJ-1, PROJ-2)` Returns users that are watchers on the issues _PROJ-1_ or _PROJ-2_.
        *   `is voter of (PROJ-1, PROJ-2)` Returns users that are voters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is commenter of (PROJ-1, PROJ-2)` Returns users that have posted a comment on the issues _PROJ-1_ or _PROJ-2_.
        *   `is transitioner of (PROJ-1, PROJ-2)` Returns users that have performed a transition on issues _PROJ-1_ or _PROJ-2_.
        *   `[propertyKey].entity.property.path is "property value"` Returns users with the entity property value.

        The list of issues can be extended as needed, as in _(PROJ-1, PROJ-2, ... PROJ-n)_. Statements can be combined using the `AND` and `OR` operators to form more complex queries, for example:

        `is assignee of PROJ AND [propertyKey].entity.property.path is "property value"`
      operationId: com.atlassian.jira.rest.v2.search.UserSearchResource.findUserKeysByQuery_get
      x-api-path-slug: api2usersearchquerykey-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: includeInactive
        description: Include inactive users in the results
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: query
        description: The search query
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Find
      - User
      - Keys
      - By
      - Query
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:configuration/{key}/state:
    put:
      summary: Update the chat:configuration state
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatConfigurationPutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatconfigurationkeystate-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: Key of the configuration module
      responses:
        200:
          description: OK
      tags:
      - Chat:configuration
      - State
  /site/{cloudId}/conversation/{conversationId}/app/module/chat:glance/{key}/state:
    put:
      summary: Update the chat:glance state
      description: Authentication required, with scope participate:conversation
      operationId: AppModuleChatGlanceStatePutHandler
      x-api-path-slug: sitecloudidconversationconversationidappmodulechatglancekeystate-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: key
        description: Key of the glance
      responses:
        200:
          description: OK
      tags:
      - Chat:glance
      - State
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