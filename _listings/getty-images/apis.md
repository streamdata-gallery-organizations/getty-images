---
name: Getty Images
x-slug: getty-images
description: Find high resolution royalty-free images, editorial stock photos, vector
  art, video footage clips and stock music licensing at the richest image search photo
  library online.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
x-kinRank: "8"
x-alexaRank: "1939"
tags: Getty Images
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Search Artist Images
  x-api-slug: getty-images
  description: Search for images by a photographer
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/artists/images
  tags: Images,Artists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3artistsimages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3artistsimages-get-openapi.md
- name: Getty Images Search Artist ImaVideosges
  x-api-slug: getty-images
  description: Search for videos by a photographer
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/artists/videos
  tags: Images,Artists,Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3artistsvideos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3artistsvideos-get-openapi.md
- name: Getty Images Get Asset Change Notifications
  x-api-slug: getty-images
  description: "# Asset Changes\r\n\r\nGet notifications about new, updated or deleted
    assets.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token
    to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n    \r\nPartner
    channels that have not been checked within the last 120 days will be removed and
    that partner will no longer be able \r\nto get change notifications from that
    channel.\r\nPartners who would like to start using the Asset Changes API again
    after a period of dormancy should contact their sales\r\nrepresentative to be
    set up again."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/asset-changes/change-sets
  tags: Images,Changes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetchangeschangesets-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetchangeschangesets-put-openapi.md
- name: Getty Images Get Asset Change Notification
  x-api-slug: getty-images
  description: "# Delete Asset Changes\r\n\r\nConfirm asset changes acknowledges receipt
    of asset changes (from the PUT asset changes endpoint).\r\n\r\n##  Quickstart\r\n\r\nYou'll
    need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/asset-changes/change-sets/{change-set-id}
  tags: Images,Changes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetchangeschangesetschangesetid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetchangeschangesetschangesetid-delete-openapi.md
- name: Getty Images Get Asset Change Channels
  x-api-slug: getty-images
  description: "# Get Partner Channels\r\n\r\nRetrieves the channel data for the partner.
    This data can be used to populate the channel_id parameter in the Put Asset Changes
    query.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token
    to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\nOnly channels
    that have been queried in the last 120 days will be included in the list of channels.\r\nPartners
    who have a channel that has been removed should contact their sales representative
    to be set up again."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/asset-changes/channels
  tags: Images,Changes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetchangeschannels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetchangeschannels-get-openapi.md
- name: Getty Images Register Assets
  x-api-slug: getty-images
  description: "# Register Assets\r\n\r\nRegisters a list of assets that a customer
    has stored in their system.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n_Note_: In
    the event of a successful query (response code 200) there will be nothing in the
    response body."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/asset-registrations
  tags: Images,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3assetregistrations-post-openapi.md
- name: Getty Images Get All Boards
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to retrieve all Boards available for a user.\r\n\r\nYou'll need
    an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boards-get-openapi.md
- name: Getty Images Create Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to create a Board by a specific id.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n**NOTE:** *The
    input to this endpoint is not sanitized in any way, so it is the responsibility
    of the client to ensure that it is properly formatted and guards against malicious
    data (for example cross-site scripting attacks or HTML injection) when accessing
    the data.*"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Images,Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boards-post-openapi.md
- name: Getty Images Delete Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to delete a Board by a specific id.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-id-delete-openapi.md
- name: Getty Images Get Board Assets
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to retrieve a Board by a specific id.\r\n\r\nYou'll need an
    API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-id-get-openapi.md
- name: Getty Images Update Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to update a Board by a specific id.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n**NOTE:** *The
    input to this endpoint is not sanitized in any way, so it is the responsibility
    of the client to ensure that it is properly formatted and guards against malicious
    data (for example cross-site scripting attacks or HTML injection) when accessing
    the data.*"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Images,Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-id-put-openapi.md
- name: Getty Images Remove Assets From Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to remove a set of assets from a board.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassets-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassets-delete-openapi.md
- name: Getty Images Add Assets to a Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to add a set of assets to a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Images,Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassets-put-openapi.md
- name: Getty Images Remove an asset from a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to remove an asset from a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassetsasset-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassetsasset-id-delete-openapi.md
- name: Getty Images Add an asset to a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place.\r\nMore information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to add an asset to a board.\r\n\r\nYou'll need an API key and
    a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassetsasset-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idassetsasset-id-put-openapi.md
- name: Getty Images Get comments from a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to retrieve all comments for a specific board.\r\n\r\nYou'll
    need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Images,Boards,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idcomments-get-openapi.md
- name: Getty Images Add a comment to a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to add a comment to a board.\r\n\r\nYou'll need an API key and a
    [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Images,Boards,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idcomments-post-openapi.md
- name: Getty Images Delete a comment from a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to delete a comment from a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments/{comment_id}
  tags: Images,Boards,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idcommentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3boardsboard-idcommentscomment-id-delete-openapi.md
- name: Getty Images Get Collections
  x-api-slug: getty-images
  description: "Use this endpoint to retrieve collections associated with your Getty
    Images account. To browse available collections see our [Image collections page](
    http://www.gettyimages.com/creative-images/collections).\r\n\r\nYou'll need an
    API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/collections
  tags: Images,Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3collections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3collections-get-openapi.md
- name: Getty Images Get Countries
  x-api-slug: getty-images
  description: "Returns a list of country objects that contains country name, two
    letter ISO abbreviation and three letter ISO abbreviation.\r\n\r\nYou'll need
    an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/countries
  tags: Images,Countries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3countries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3countries-get-openapi.md
- name: Getty Images Get Downloads
  x-api-slug: getty-images
  description: "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll
    need an API key and access token to use this resource. Please see our [Getting
    Started](http://developers.gettyimages.com/en/getting-started.html) page for more
    information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint requires
    being a Getty Images customer to limit your results to only assets that you have
    a license to use, \r\nyou need to also include an authorization token in the header
    of your request. \r\nPlease consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/downloads
  tags: Images,Downloads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3downloads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3downloads-get-openapi.md
- name: Getty Images Download an image
  x-api-slug: getty-images
  description: "Use this endpoint to generate download URLs and related data for images
    you are authorized to download.\r\n\r\nMost product offerings have enforced periodic
    download limits such as monthly, weekly, and daily. When this operation executes,
    the count of allowed downloads is decremented by one for the product offering.
    Once the download limit is reached for a given product offering, no further downloads
    may be requested for that product offering until the next download period.\r\n\r\nThe
    download limit for a given download period is covered in your product agreement
    established with Getty Images.\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n## Auto Downloads\r\nThe
    `auto_download` request query parameter specifies whether to automatically download
    the image.\r\n\r\nIf the `auto_download` request query parameter is set to _true_,
    the API will return an HTTP status code 303 *See Other*.\u2002Your client code
    will need to process this response and redirect to the URI specified in the *Location*
    header to enable you to automatically download the file. The redirection workflow
    follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
    Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
    the `auto_download` request query parameter is set to false, the API will return
    a HTTP status code 200, along with the URI in the response body which can be used
    to download the image. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/downloads/images/{id}
  tags: Images,Downloads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3downloadsimagesid-post-openapi.md
- name: Getty Images Download a video
  x-api-slug: getty-images
  description: "Use this endpoint to generate download URLs and related data for videos
    you are authorized to download.\r\n\r\nMost product offerings have enforced periodic
    download limits such as monthly, weekly, and daily. When this operation executes,
    the count of allowed downloads is decremented by one for the product offering.
    Once the download limit is reached for a given product offering, no further downloads
    may be requested for that product offering until the next download period.\r\n\r\nThe
    download limit for a given download period is covered in your product agreement
    established with Getty Images.\r\n\r\nYou'll need an API key and a [Resource Owner
    Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n## Auto Downloads\r\nThe
    `auto_download` request query parameter specifies whether to automatically download
    the video.\r\n\r\nIf the `auto_download` request query parameter is set to _true_,
    the API will return an HTTP status code 303 *See Other*.\u2002Your client code
    will need to process this response and redirect to the URI specified in the *Location*
    header to enable you to automatically download the file. The redirection workflow
    follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
    Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
    the `auto_download` request query parameter is set to false, the API will return
    a HTTP status code 200, along with the URI in the response body which can be used
    to download the video. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
    Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/downloads/videos/{id}
  tags: Images,Downloads,Videos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3downloadsvideosid-post-openapi.md
- name: Getty Images Get metadata for multiple events
  x-api-slug: getty-images
  description: "This endpoint returns the detailed event metadata for all specified
    events. Getty Images news, sports and entertainment photographers and\r\nvideographers
    cover editorially relevant events occurring around the world.  All images or video
    clips produced in association with \r\nan event, are assigned the same EventID.
    EventIDs are part of the meta-data returned in SearchForImages Results. Only content
    \r\nproduced under a Getty Images brand name (Getty Images News, Getty Images
    Sports, Getty Images Entertainment, Film Magic, Wire Image) \r\nwill be consistently
    assigned an EventID. The Event framework may also be used to group similar content,
    such as \r\n\"Hats from the Royal Wedding\" or \"Odd-ballOffbeat images of the
    week\". \r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/events
  tags: Images,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3events-get-openapi.md
- name: Getty Images Get metadata for a single event
  x-api-slug: getty-images
  description: "This endpoint returns the detailed event metadata for a specified
    event. Getty Images news, sports and entertainment \r\nphotographers and videographers
    cover editorially relevant events occurring around the world.  \r\nAll images
    or video clips produced in association with an event, are assigned the same EventID.
    \r\nEventIDs are part of the meta-data returned in SearchForImages Results. Only
    content produced under a Getty Images \r\nbrand name (Getty Images News, Getty
    Images Sports, Getty Images Entertainment, Film Magic, Wire Image) will be \r\nconsistently
    assigned an EventID. The Event framework may also be used to group similar content,
    such as \r\n\"Hats from the Royal Wedding\" or \"Odd-ballOffbeat images of the
    week\". \r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/events/{id}
  tags: Images,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3eventsid-get-openapi.md
- name: Getty Images Get Images
  x-api-slug: getty-images
  description: "This endpoint returns the detailed image metadata for all specified
    images. Due to a wide variety of available image resolutions,\r\nthe images are
    grouped into a handful of size categories for simplicity. \r\n\r\nYou'll need
    an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    \r\npage for more information on how to sign up for an API key. \r\n\r\n## Working
    with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
    to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
    Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields value
    represents a small batch of metadata fields that are often used to build \r\nsearch
    response results. The following fields are provided for every image in your result
    set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
    \   [\r\n        \"artist\",\r\n        \"asset_family\",\r\n        \"caption\",\r\n
    \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
    \       \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n
    \   ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query
    string parameter fields value represents a large batch of metadata fields that
    are often used to build a \r\ndetailed view of images. The following fields are
    provided for every image in your result set when you include **detail_set** in
    your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"allowed_use\",\r\n
    \       \"artist\", \r\n        \"artist_title\", \r\n        \"asset_family\",\r\n
    \       \"call_for_image\",\r\n        \"caption\", \r\n        \"city\",\r\n
    \       \"collection_code\",\r\n        \"collection_id\", \r\n        \"collection_name\",\r\n
    \       \"color_type\", \r\n        \"copyright\", \r\n        \"country\", \r\n
    \       \"credit_line\", \r\n        \"date_created\", \r\n        \"date_submitted\",\r\n
    \       \"download_sizes\", \r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n
    \       \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
    \       \"orientation\",\r\n        \"prestige\",\r\n        \"product_types\",\r\n
    \       \"quality_rank\",\r\n        \"referral_destinations\",\r\n        \"state_province\",
    \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution\r\nfiles that are most frequently
    used to build a UI displaying search results. The following fields are provided
    for every image \r\nin your result set when you include **display_set** in your
    request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n##
    Request Usage Considerations\r\n\r\n- Specifying the \"entity_details\" response
    field can have significant performance implications. The field should be used
    only when necessary."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/images
  tags: Images
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3images-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3images-get-openapi.md
- name: Getty Images Get Image
  x-api-slug: getty-images
  description: "This endpoint returns the detailed image metadata for a specified
    image. Due to a wide variety of available image resolutions, \r\nthe images are
    grouped into a handful of size categories for simplicity. \r\n\r\nYou'll need
    an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    \r\npage for more information on how to sign up for an API key. \r\n \r\n## Working
    with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
    to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
    Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields value
    represents a small batch of metadata fields that\r\nare often used to build search
    response results. The following fields are provided for every image in your\r\nresult
    set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
    \   [\r\n        \"artist\",\r\n        \"asset_family\",\r\n        \"caption\",\r\n
    \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
    \       \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n
    \   ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query
    string parameter fields value represents a large batch of metadata fields that
    are \r\noften used to build a detailed view of images. The following fields are
    provided for every image in your \r\nresult set when you include **detail_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"allowed_use\",\r\n
    \       \"artist\", \r\n        \"artist_title\", \r\n        \"asset_family\",\r\n
    \       \"call_for_image\",\r\n        \"caption\", \r\n        \"city\",\r\n
    \       \"collection_code\",\r\n        \"collection_id\", \r\n        \"collection_name\",\r\n
    \       \"color_type\", \r\n        \"copyright\", \r\n        \"country\", \r\n
    \       \"credit_line\", \r\n        \"date_created\", \r\n        \"date_submitted\",\r\n
    \       \"download_sizes\", \r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n
    \       \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
    \       \"orientation\",\r\n        \"prestige\",\r\n        \"product_types\",\r\n
    \       \"quality_rank\",\r\n        \"referral_destinations\",\r\n        \"state_province\",
    \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low\r\nresolution files that are most frequently
    used to build a UI displaying search results. The following fields are provided
    \r\nfor every image in your result set when you include **display_set** in your
    request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n##
    Request Usage Considerations\r\n\r\n- Specifying the \"entity_details\" response
    field can have significant performance implications. The field should be used
    only when necessary."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/images/{id}
  tags: Images
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3imagesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3imagesid-get-openapi.md
- name: Getty Images Search Similar Images
  x-api-slug: getty-images
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/images/{id}/similar
  tags: Images,Similar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3imagesidsimilar-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3imagesidsimilar-get-openapi.md
- name: Getty Images Get Products
  x-api-slug: getty-images
  description: "This endpoint returns all products available to the username used
    during authentication. As such, this endpoint requires the use of\r\na fully authorized
    access_token. The product data can then be used as search filters, restricting
    results to images from a specific product.\r\n\r\nYou'll need an API key and access
    token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/products
  tags: Images,Products
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3products-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3products-get-openapi.md
- name: Getty Images Get Purchased Images
  x-api-slug: getty-images
  description: "This endpoint returns a list of all assets purchased on gettyimages.com
    by the username used for authentication. \r\nUse of this endpoint requires configuration
    changes to your API key. \r\nPlease contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)
    to learn more.\r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/purchased-assets
  tags: Images,Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3purchasedassets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3purchasedassets-get-openapi.md
- name: Getty Images Get Previously Purchased Images
  x-api-slug: getty-images
  description: "This endpoint returns a list of all images purchased on gettyimages.com
    by the username used for authentication.\r\nUse of this endpoint requires configuration
    changes to your API key. Please contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)\r\nto
    learn more.\r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/purchased-images
  tags: Images,Purchases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3purchasedimages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3purchasedimages-get-openapi.md
- name: Getty Images Search for events
  x-api-slug: getty-images
  description: "Use this endpoint to search Getty Images news, sports and entertainment
    events. Getty Images photographers and videographers cover editorially relevant
    events occurring around the world.  All images or video clips produced in association
    with an event, are assigned the same EventID. EventIDs are part of the meta-data
    returned in Search Results. Only content produced under a Getty Images brand name
    (Getty Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
    Wire Image) will be consistently assigned an EventID. The Event framework may
    also be used to group similar content, such as \"Hats from the Royal Wedding\"
    or \"Odd-ballOffbeat images of the week\".   \r\n\r\nYou'll need an API key and
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n\r\nYou can
    show different information in the response by specifying values on the \"fields\"
    parameter (see details below).\r\nYou can search with only an API key, and that
    will give you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/events
  tags: Images,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchevents-get-openapi.md
- name: Getty Images Search Images
  x-api-slug: getty-images
  description: Use this endpoint to search over a blend of our contemporary stock
    photos, illustrations, archival images, editorial photos, illustrations and archival
    images.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/images
  tags: Images,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimages-get-openapi.md
- name: Getty Images Search for creative images only
  x-api-slug: getty-images
  description: "Use this endpoint to search our contemporary stock photos, illustrations
    and archival images.\r\n\r\nYou'll need an API key and access token to use this
    resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    \r\npage for more information on how to sign up for an API key. \r\n \r\nYou can
    show different information in the response by specifying values on the \"fields\"
    parameter (see details below).\r\nYou can search with only an API key, and that
    will give you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to \r\nbuild search response results. The
    following fields are provided for every image in your result set when you include
    **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\": \r\n    [\r\n
    \       \"asset_family\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n
    \   ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query
    string parameter fields value represents a large batch of metadata fields that
    are often used to \r\nbuild a detailed view of images. The following fields are
    provided for every image in your result set when you include **detail_set** in
    your request.\r\n\r\n```\r\n{\r\n    \"images\": \r\n    [\r\n        \"allowed_use\",\r\n
    \       \"artist\",\r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
    \       \"collection_name\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
    \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n        \"graphical_style\",\r\n
    \       \"license_model\",\r\n        \"max_dimensions\",\r\n        \"orientation\",\r\n
    \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
    \       \"title\"\r\n    ]\r\n]\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution\r\nfiles that are most frequently
    used to build a UI displaying search results. The following fields are provided
    for every image \r\nin your result set when you include **display_set** in your
    request.\r\n\r\n```Go\r\n{\r\n    \"images\": \r\n    [\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/images/creative
  tags: Images,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimagescreative-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimagescreative-get-openapi.md
- name: Getty Images Search Images by Image
  x-api-slug: getty-images
  description: "Allows searching for similar creative images by passing the URL to
    an existing image.\r\n\r\nBefore calling the search by image endpoint, an image
    must be uploaded to a specific AWS S3 bucket. The bucket name is `search-by-image.s3.amazonaws.com`.\r\nFor
    example, using cURL:\r\n```sh\r\ncurl -i -X PUT https://search-by-image.s3.amazonaws.com/my-test-image.jpg
    -H \"Content-Type: image/jpeg\" --data-binary \"@testimage.jpg\"\r\n```\r\n\r\nUploads
    can be overwritten if the names are the same, so using a prefix like the API Key,
    application name or company name would help keep that\r\nfrom happening.\r\n\r\nOnce
    the image has been uploaded, use the full URL in the `image_url` parameter, e.g.
    `image_url=https://search-by-image.s3.amazonaws.com/my-test-image.jpg`.\r\n\r\nSubsequent
    searches for the same image can be executed using the `image_fingerprint` that
    is returned by the inital search."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/images/creative/by-image
  tags: Images,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimagescreativebyimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimagescreativebyimage-get-openapi.md
- name: Getty Images Search Editorial Images
  x-api-slug: getty-images
  description: Use this endpoint to search our editorial stock photos, illustrations
    and archival images.  Editorial images represent newsworthy events or illustrate
    matters of general interest, such as news, sport and entertainment and are generally
    intended for editorial use.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/images/editorial
  tags: Images,Search,Editorial
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimageseditorial-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchimageseditorial-get-openapi.md
- name: Getty Images Search Editorial Videos
  x-api-slug: getty-images
  description: "Use this endpoint to search over a blend of our premium stock, contemporary
    4K and HD footage, celebrities, news, newsmakers, entertainment, events and archival
    videos.\r\n\r\nYou'll need an API key and access token to use this resource. Please
    see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n\r\nYou can
    show different information in the response by specifying values on the \"fields\"
    parameter (see details below).\r\nYou can search with only an API key, and that
    will give you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search response results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a detailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
    \   [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"era\",\r\n
    \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
    \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
    \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution files that are most frequently used
    to build a UI displaying search results. The following fields are provided for
    every video in your result set when you include **display_set** in your request.\r\n\r\n```\r\n{\r\n
    \   \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n
    \               \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\":
    \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n
    \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
    Specifying the \"entity_details\" response field can have significant performance
    implications. The field should be used only when necessary."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/videos
  tags: Images,Search,Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchvideos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchvideos-get-openapi.md
- name: Getty Images Search for creative videos
  x-api-slug: getty-images
  description: "Use this endpoint to search premium stock video, from archival film
    to contemporary 4K and HD footage.\r\n\r\nYou'll need an API key and access token
    to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key.\r\n\r\nYou can show different
    information in the response by specifying values on the \"fields\" parameter (see
    details below).\r\nYou can search with only an API key, and that will give you
    search results that are equivalent to doing a search on the GettyImages.com site
    without\r\nbeing logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only \r\nassets
    that you have a license to use, you need to also include an authorization token
    in the header of your request.\r\nPlease consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search\r\nresponse results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\": \r\n    [\r\n        \"asset_family\",
    \r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a \r\ndetailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":
    \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",
    \r\n        \"caption\", \r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\", \r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"era\",\r\n
    \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
    \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
    \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution files \r\nthat are most frequently
    used to build a UI displaying search results. The following fields are provided
    for every video in your result \r\nset when you include **display_set** in your
    request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/videos/creative
  tags: Images,Search,Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchvideoscreative-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchvideoscreative-get-openapi.md
- name: Getty Images Search for editorial videos
  x-api-slug: getty-images
  description: "Use this endpoint to search current and archival video clips of celebrities,
    newsmakers, and events.\r\n\r\nYou'll need an API key and access token to use
    this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\nYou can show
    different information in the response by specifying values on the \"fields\" parameter
    (see details below).\r\nYou can search with only an API key, and that will give
    you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search response results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\": \r\n    [\r\n        \"asset_family\",
    \r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a detailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":
    \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",
    \r\n        \"caption\", \r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\", \r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"era\",\r\n
    \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
    \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
    \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution files that are most frequently used
    to build a UI displaying search results. The following fields are provided for
    every video in your result set when you include **display_set** in your request.\r\n\r\n```\r\n{\r\n
    \   \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n
    \               \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\":
    \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n
    \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
    Specifying the \"entity_details\" response field can have significant performance
    implications. The field should be used only when necessary."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/search/videos/editorial
  tags: Images,Search,Videos,Editoria
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchvideoseditorial-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3searchvideoseditorial-get-openapi.md
- name: Getty Images Reports Usage Batches
  x-api-slug: getty-images
  description: "# Report Usage\r\n\r\nUse this endpoint to report the usages of a
    set of assets. The count of assets submitted in a single batch to this endpoint
    is limited to 1000. Note that all asset Ids specified must be valid or the operation
    will fail causing no usages to be recorded. In this case, you will need to remove
    the invalid asset Ids from the query request and re-submit the query.\r\n\r\n##
    \ Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key. \r\n\r\n\r\n_Note_:
    Date of use can be in any unambiguous date format."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/usage-batches/{id}
  tags: Images,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3usagebatchesid-put-openapi.md
- name: Getty Images Get Videos Metadatata
  x-api-slug: getty-images
  description: "Use this endpoint to return detailed video metadata for all the specified
    video ids.\r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\nYou can show
    different information in the response by specifying values on the \"fields\" parameter
    (see details below).\r\nYou can search with only an API key, and that will give
    you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search response results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\": \r\n    [\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a detailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":
    \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"download_sizes\",\r\n
    \       \"era\",\r\n        \"license_model\",\r\n        \"mastered_to\",\r\n
    \       \"originally_shot_on\",\r\n        \"product_types\",\r\n        \"shot_speed\",\r\n
    \       \"source\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display
    Fields Set\r\n\r\nThe **display_set** query string parameter fields value represents
    the fields that provide you with URLs for the low resolution files that are most
    frequently used to build a UI displaying search results. The following fields
    are provided for every video in your result set when you include **display_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n##
    Request Usage Considerations\r\n\r\n- Specifying the \"entity_details\" response
    field can have significant performance implications. The field should be used
    only when necessary."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/videos
  tags: Images,Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3videos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3videos-get-openapi.md
- name: Getty Images Get Video Metadatata
  x-api-slug: getty-images
  description: "Use this endpoint to return detailed video metadata for the specified
    video id.\r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\nYou can show
    different information in the response by specifying values on the \"fields\" parameter
    (see details below).\r\nYou can search with only an API key, and that will give
    you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search response results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a detailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
    \   [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"download_sizes\",\r\n
    \       \"era\",\r\n        \"license_model\",\r\n        \"mastered_to\",\r\n
    \       \"originally_shot_on\",\r\n        \"product_types\",\r\n        \"shot_speed\",\r\n
    \       \"source\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display
    Fields Set\r\n\r\nThe **display_set** query string parameter fields value represents
    the fields that provide you with URLs for the low resolution files that are most
    frequently used to build a UI displaying search results. The following fields
    are provided for every video in your result set when you include **display_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n##
    Request Usage Considerations\r\n\r\n- Specifying the \"entity_details\" response
    field can have significant performance implications. The field should be used
    only when necessary."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/videos/{id}
  tags: Images,Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3videosid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3videosid-get-openapi.md
- name: Getty Images Get Similar Videos
  x-api-slug: getty-images
  description: Get videos similar to a video by supplying one video id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/videos/{id}/similar
  tags: Images,Videos,Similiar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3videosidsimilar-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/v3videosidsimilar-get-openapi.md
- name: Getty Images
  x-api-slug: getty-images
  description: Find high resolution royalty-free images, editorial stock photos, vector
    art, video footage clips and stock music licensing at the richest image search
    photo library online.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Getty Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/getty-images/master/_listings/getty-images/openapi.md
x-common:
- type: x-authentication
  url: https://github.com/gettyimages/connect#authentication
- type: x-base
  url: https://connect.gettyimages.com/
- type: x--net-sdk
  url: https://github.com/gettyimages/connect_sdk_csharp
- type: x-crunchbase
  url: https://crunchbase.com/organization/gettyimages
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ge-tt
- type: x-developer
  url: http://api.gettyimages.com/
- type: x-documentation
  url: https://api.gettyimages.com/swagger/ui/index.html
- type: x-email
  url: privacy@gettyimages.com
- type: x-email
  url: sales@gettyimages.com
- type: x-email
  url: copyright@gettyimages.com
- type: x-embeddable
  url: https://github.com/gettyimages/connect#oembed
- type: x-forum
  url: http://api.gettyimages.com/forum
- type: x-getting-started
  url: https://github.com/gettyimages/connect#getting-started
- type: x-github
  url: https://github.com/gettyimages
- type: x-java-sdk
  url: https://github.com/gettyimages/connect_sdk_java
- type: x-node-js-sdk
  url: https://github.com/gettyimages/connect_sdk_nodejs
- type: x-objectivec-sdk
  url: https://github.com/gettyimages/connect_sdk_objective-c
- type: x-php-sdk
  url: https://github.com/gettyimages/connect_sdk_php
- type: x-pricing
  url: http://www.gettyimages.com/subscribe
- type: x-ruby-sdk
  url: https://github.com/gettyimages/connect_sdk_ruby
- type: x-twitter
  url: https://twitter.com/GettyImages
- type: x-website
  url: http://www.gettyimages.com/
- type: x-website
  url: http://gettyimages.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---