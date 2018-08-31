---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Search Similar Images
  description: "This endpoint will search our asset database for images similar to
    the specified asset id. Due to a wide variety of available \r\nimage resolutions,
    the images are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
    need an API key and access token to use this resource. Please see our [Getting
    Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage for
    more information on how to sign up for an API key. \r\n\r\n## Working with Fields
    Sets\r\n\r\nFields sets are used in the **fields** request parameter to receive
    a suite of metadata fields. The following fields sets are available:\r\n\r\n####
    Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields value
    represents a small batch of metadata fields that are often used to build\r\nsearch
    response results. The following fields are provided for every image in your result
    set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
    \   [\r\n        \"asset_family\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ]\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n
    \   ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query
    string parameter fields value represents a large batch of metadata fields that
    are often used to build a \r\ndetailed view of images. The following fields are
    provided for every image in your result set when you include **detail_set** in
    your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"allowed_use\",\r\n
    \       \"artist\",\r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
    \       \"collection_name\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
    \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n        \"graphical_style\",\r\n
    \       \"license_model\",\r\n        \"max_dimensions\",\r\n        \"orientation\",\r\n
    \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
    \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution files \r\nthat are most frequently
    used to build a UI displaying search results. The following fields are provided
    for every image in your result\r\nset when you include **display_set** in your
    request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
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
  /v3/boards/{board_id}/assets/{asset_id}:
    delete:
      summary: Remove an asset from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to remove an asset from a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_RemoveAsset
      x-api-path-slug: v3boardsboard-idassetsasset-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: path
        name: asset_id
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
      summary: Add an asset to a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place.\r\nMore information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to add an asset to a board.\r\n\r\nYou'll need an API key
        and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddAsset
      x-api-path-slug: v3boardsboard-idassetsasset-id-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: path
        name: asset_id
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
  /v3/boards/{board_id}/comments:
    get:
      summary: Get comments from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve all comments for a specific board.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetComments
      x-api-path-slug: v3boardsboard-idcomments-get
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
      - Comments
    post:
      summary: Add a comment to a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to add a comment to a board.\r\n\r\nYou'll need an API key and
        a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddComment
      x-api-path-slug: v3boardsboard-idcomments-post
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
        name: comment
        description: Comment to be added to the board
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
  /v3/boards/{board_id}/comments/{comment_id}:
    delete:
      summary: Delete a comment from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to delete a comment from a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_DeleteComment
      x-api-path-slug: v3boardsboard-idcommentscomment-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      - in: path
        name: comment_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
  /v3/collections:
    get:
      summary: Get Collections
      description: "Use this endpoint to retrieve collections associated with your
        Getty Images account. To browse available collections see our [Image collections
        page]( http://www.gettyimages.com/creative-images/collections).\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key."
      operationId: Collections_GetCollections
      x-api-path-slug: v3collections-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Collections
  /v3/countries:
    get:
      summary: Get Countries
      description: "Returns a list of country objects that contains country name,
        two letter ISO abbreviation and three letter ISO abbreviation.\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key."
      operationId: Countries_GetCountries
      x-api-path-slug: v3countries-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Countries
  /v3/downloads:
    get:
      summary: Get Downloads
      description: "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint
        requires being a Getty Images customer to limit your results to only assets
        that you have a license to use, \r\nyou need to also include an authorization
        token in the header of your request. \r\nPlease consult our [Authorization
        FAQ](http://developers.gettyimages.com/en/authorization-faq.html) for more
        information on authorization tokens."
      operationId: Downloads_GetDownloads
      x-api-path-slug: v3downloads-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: company_downloads
        description: If specified, returns the list of previously downloaded images
          for all users in your company
      - in: query
        name: end_date
        description: If specified, select assets downloaded on or before this date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: product_type
        description: Specifies product type to be included in the previous download
          results
      - in: query
        name: start_date
        description: If specified, select assets downloaded on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
  /v3/downloads/images/{id}:
    post:
      summary: Download an image
      description: "Use this endpoint to generate download URLs and related data for
        images you are authorized to download.\r\n\r\nMost product offerings have
        enforced periodic download limits such as monthly, weekly, and daily. When
        this operation executes, the count of allowed downloads is decremented by
        one for the product offering. Once the download limit is reached for a given
        product offering, no further downloads may be requested for that product offering
        until the next download period.\r\n\r\nThe download limit for a given download
        period is covered in your product agreement established with Getty Images.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n## Auto
        Downloads\r\nThe `auto_download` request query parameter specifies whether
        to automatically download the image.\r\n\r\nIf the `auto_download` request
        query parameter is set to _true_, the API will return an HTTP status code
        303 *See Other*.???Your client code will need to process this response and
        redirect to the URI specified in the *Location* header to enable you to automatically
        download the file. The redirection workflow follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
        Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
        the `auto_download` request query parameter is set to false, the API will
        return a HTTP status code 200, along with the URI in the response body which
        can be used to download the image. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
      operationId: Downloads_PostDownloads
      x-api-path-slug: v3downloadsimagesid-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the image
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: file_type
        description: File Type expressed with three character file extension
      - in: query
        name: height
        description: Specifies the pixel height of the particular image to download
      - in: path
        name: id
        description: Id of image to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: product_type
        description: Product type
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
  /v3/downloads/videos/{id}:
    post:
      summary: Download a video
      description: "Use this endpoint to generate download URLs and related data for
        videos you are authorized to download.\r\n\r\nMost product offerings have
        enforced periodic download limits such as monthly, weekly, and daily. When
        this operation executes, the count of allowed downloads is decremented by
        one for the product offering. Once the download limit is reached for a given
        product offering, no further downloads may be requested for that product offering
        until the next download period.\r\n\r\nThe download limit for a given download
        period is covered in your product agreement established with Getty Images.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n## Auto
        Downloads\r\nThe `auto_download` request query parameter specifies whether
        to automatically download the video.\r\n\r\nIf the `auto_download` request
        query parameter is set to _true_, the API will return an HTTP status code
        303 *See Other*.???Your client code will need to process this response and
        redirect to the URI specified in the *Location* header to enable you to automatically
        download the file. The redirection workflow follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
        Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
        the `auto_download` request query parameter is set to false, the API will
        return a HTTP status code 200, along with the URI in the response body which
        can be used to download the video. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
      operationId: Downloads_PostVideoDownloads
      x-api-path-slug: v3downloadsvideosid-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the video
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of video to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: size
        description: Specifies the size to be downloaded
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
      - Videos
  /v3/events:
    get:
      summary: Get metadata for multiple events
      description: "This endpoint returns the detailed event metadata for all specified
        events. Getty Images news, sports and entertainment photographers and\r\nvideographers
        cover editorially relevant events occurring around the world.  All images
        or video clips produced in association with \r\nan event, are assigned the
        same EventID. EventIDs are part of the meta-data returned in SearchForImages
        Results. Only content \r\nproduced under a Getty Images brand name (Getty
        Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
        Wire Image) \r\nwill be consistently assigned an EventID. The Event framework
        may also be used to group similar content, such as \r\n\"Hats from the Royal
        Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an
        API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Events_GetBatch
      x-api-path-slug: v3events-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: query
        name: ids
        description: A comma separated list of event ids
      responses:
        200:
          description: OK
      tags:
      - Images
      - Events
  /v3/events/{id}:
    get:
      summary: Get metadata for a single event
      description: "This endpoint returns the detailed event metadata for a specified
        event. Getty Images news, sports and entertainment \r\nphotographers and videographers
        cover editorially relevant events occurring around the world.  \r\nAll images
        or video clips produced in association with an event, are assigned the same
        EventID. \r\nEventIDs are part of the meta-data returned in SearchForImages
        Results. Only content produced under a Getty Images \r\nbrand name (Getty
        Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
        Wire Image) will be \r\nconsistently assigned an EventID. The Event framework
        may also be used to group similar content, such as \r\n\"Hats from the Royal
        Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an
        API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Events_Get
      x-api-path-slug: v3eventsid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: path
        name: id
        description: An event id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Events
  /v3/images:
    get:
      summary: Get Images
      description: "This endpoint returns the detailed image metadata for all specified
        images. Due to a wide variety of available image resolutions,\r\nthe images
        are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage
        for more information on how to sign up for an API key. \r\n\r\n## Working
        with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
        to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that are often used to build
        \r\nsearch response results. The following fields are provided for every image
        in your result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"artist\",\r\n        \"asset_family\",\r\n
        \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
        \       \"collection_name\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe
        **detail_set** query string parameter fields value represents a large batch
        of metadata fields that are often used to build a \r\ndetailed view of images.
        The following fields are provided for every image in your result set when
        you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"allowed_use\",\r\n        \"artist\", \r\n        \"artist_title\",
        \r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",
        \r\n        \"city\",\r\n        \"collection_code\",\r\n        \"collection_id\",
        \r\n        \"collection_name\",\r\n        \"color_type\", \r\n        \"copyright\",
        \r\n        \"country\", \r\n        \"credit_line\", \r\n        \"date_created\",
        \r\n        \"date_submitted\",\r\n        \"download_sizes\", \r\n        \"editorial_segments\",\r\n
        \       \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"orientation\",\r\n        \"prestige\",\r\n
        \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
        \       \"state_province\", \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution\r\nfiles
        that are most frequently used to build a UI displaying search results. The
        following fields are provided for every image \r\nin your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Images_GetBatch
      x-api-path-slug: v3images-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: ids
        description: Specifies one or more image ids to return
      responses:
        200:
          description: OK
      tags:
      - Images
  /v3/images/{id}:
    get:
      summary: Get Image
      description: "This endpoint returns the detailed image metadata for a specified
        image. Due to a wide variety of available image resolutions, \r\nthe images
        are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage
        for more information on how to sign up for an API key. \r\n \r\n## Working
        with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
        to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that\r\nare often used to
        build search response results. The following fields are provided for every
        image in your\r\nresult set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"artist\",\r\n        \"asset_family\",\r\n
        \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
        \       \"collection_name\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe
        **detail_set** query string parameter fields value represents a large batch
        of metadata fields that are \r\noften used to build a detailed view of images.
        The following fields are provided for every image in your \r\nresult set when
        you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"allowed_use\",\r\n        \"artist\", \r\n        \"artist_title\",
        \r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",
        \r\n        \"city\",\r\n        \"collection_code\",\r\n        \"collection_id\",
        \r\n        \"collection_name\",\r\n        \"color_type\", \r\n        \"copyright\",
        \r\n        \"country\", \r\n        \"credit_line\", \r\n        \"date_created\",
        \r\n        \"date_submitted\",\r\n        \"download_sizes\", \r\n        \"editorial_segments\",\r\n
        \       \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"orientation\",\r\n        \"prestige\",\r\n
        \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
        \       \"state_province\", \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low\r\nresolution
        files that are most frequently used to build a UI displaying search results.
        The following fields are provided \r\nfor every image in your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Images_Get
      x-api-path-slug: v3imagesid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: path
        name: id
        description: An image id
      responses:
        200:
          description: OK
      tags:
      - Images
  /v3/images/{id}/similar:
    get:
      summary: Search Similar Images
      description: "This endpoint will search our asset database for images similar
        to the specified asset id. Due to a wide variety of available \r\nimage resolutions,
        the images are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage
        for more information on how to sign up for an API key. \r\n\r\n## Working
        with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
        to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that are often used to build\r\nsearch
        response results. The following fields are provided for every image in your
        result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"thumb\"\r\n            }\r\n        ]\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a \r\ndetailed view of images. The following fields are provided for every
        image in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":
        \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n
        \       \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"orientation\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n
        \       \"referral_destinations\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution
        files \r\nthat are most frequently used to build a UI displaying search results.
        The following fields are provided for every image in your result\r\nset when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```"
      operationId: Images_GetSimilarImages
      x-api-path-slug: v3imagesidsimilar-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: path
        name: id
        description: Identifies an existing image
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
      - Similar
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