---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Add Assets to a Board
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to add a set of assets to a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  version: 1.0.0
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/artists/images:
    get:
      summary: Search Artist Images
      description: Search for images by a photographer
      operationId: Artists_GetImagesByArtist
      x-api-path-slug: v3artistsimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: artist_name
        description: Name of artist for desired images
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Comma separated list of fields
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Artists
  /v3/artists/videos:
    get:
      summary: Search Artist ImaVideosges
      description: Search for videos by a photographer
      operationId: Artists_GetVideosByArtist
      x-api-path-slug: v3artistsvideos-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: artist_name
        description: Name of artist for desired images
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Comma separated list of fields
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Artists
      - Videos
  /v3/asset-changes/change-sets:
    put:
      summary: Get Asset Change Notifications
      description: "# Asset Changes\r\n\r\nGet notifications about new, updated or
        deleted assets.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a
        [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n    \r\nPartner
        channels that have not been checked within the last 120 days will be removed
        and that partner will no longer be able \r\nto get change notifications from
        that channel.\r\nPartners who would like to start using the Asset Changes
        API again after a period of dormancy should contact their sales\r\nrepresentative
        to be set up again."
      operationId: AssetChanges_PutAssetChanges
      x-api-path-slug: v3assetchangeschangesets-put
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: batch_size
        description: Specifies the number of assets to return
      - in: query
        name: channel_id
        description: Specifies the id of the channel for the asset data
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-changes/change-sets/{change-set-id}:
    delete:
      summary: Get Asset Change Notification
      description: "# Delete Asset Changes\r\n\r\nConfirm asset changes acknowledges
        receipt of asset changes (from the PUT asset changes endpoint).\r\n\r\n##
        \ Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: AssetChanges_DeleteAssetChanges
      x-api-path-slug: v3assetchangeschangesetschangesetid-delete
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: change-set-id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-changes/channels:
    get:
      summary: Get Asset Change Channels
      description: "# Get Partner Channels\r\n\r\nRetrieves the channel data for the
        partner. This data can be used to populate the channel_id parameter in the
        Put Asset Changes query.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key
        and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\nOnly channels
        that have been queried in the last 120 days will be included in the list of
        channels.\r\nPartners who have a channel that has been removed should contact
        their sales representative to be set up again."
      operationId: AssetChanges_GetPartnerChannel
      x-api-path-slug: v3assetchangeschannels-get
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-registrations:
    post:
      summary: Register Assets
      description: "# Register Assets\r\n\r\nRegisters a list of assets that a customer
        has stored in their system.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n_Note_:
        In the event of a successful query (response code 200) there will be nothing
        in the response body."
      operationId: AssetRegistration_Register
      x-api-path-slug: v3assetregistrations-post
      parameters:
      - in: body
        name: request
        description: Specify JSON containing an array of asset ids to register
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Registrations
  /v3/boards:
    get:
      summary: Get All Boards
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve all Boards available for a user.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetAllBoards
      x-api-path-slug: v3boards-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: board_relationship
        description: Search for boards the user owns or has been invited to as an
          editor
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: pageSize
        description: Request number of boards to return in each page
      - in: query
        name: sort_order
        description: Sort the list of boards by last update date or name
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    post:
      summary: Create Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to create a Board by a specific id.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\n**NOTE:**
        *The input to this endpoint is not sanitized in any way, so it is the responsibility
        of the client to ensure that it is properly formatted and guards against malicious
        data (for example cross-site scripting attacks or HTML injection) when accessing
        the data.*"
      operationId: Boards_CreateBoard
      x-api-path-slug: v3boards-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: body
        name: new_board
        description: Specify a name and description of the board to create (name is
          required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
  /v3/boards/{board_id}:
    delete:
      summary: Delete Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to delete a Board by a specific id.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_DeleteBoard
      x-api-path-slug: v3boardsboard-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    get:
      summary: Get Board Assets
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve a Board by a specific id.\r\n\r\nYou'll need
        an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetBoard
      x-api-path-slug: v3boardsboard-id-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    put:
      summary: Update Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to update a Board by a specific id.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\n**NOTE:**
        *The input to this endpoint is not sanitized in any way, so it is the responsibility
        of the client to ensure that it is properly formatted and guards against malicious
        data (for example cross-site scripting attacks or HTML injection) when accessing
        the data.*"
      operationId: Boards_UpdateBoard
      x-api-path-slug: v3boardsboard-id-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      - in: body
        name: board_info
        description: Specify a new name and description for the board (name is required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
  /v3/boards/{board_id}/assets:
    delete:
      summary: Remove Assets From Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to remove a set of assets from a board.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_RemoveAssets
      x-api-path-slug: v3boardsboard-idassets-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: asset_ids
        description: List the assets to be removed from the board
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    put:
      summary: Add Assets to a Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to add a set of assets to a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddAssets
      x-api-path-slug: v3boardsboard-idassets-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: body
        name: board_assets
        description: List assets to add to the board
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
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