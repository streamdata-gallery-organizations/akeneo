---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API family
  description: Family.
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/assets/paint:
    get:
      summary: asset (2.1 only)
      description: Assuming that the given code is the code of an existing asset
      operationId: RestV1AssetsPaintGet
      x-api-path-slug: restv1assetspaint-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - (2
      - "1"
      - Only)
    patch:
      summary: asset (2.1 only)
      description: Asset (2.1 only).
      operationId: RestV1AssetsPaintPatch
      x-api-path-slug: restv1assetspaint-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - (2
      - "1"
      - Only)
  /rest/v1/assets:
    get:
      summary: assets (2.1 only)
      description: Assets (2.1 only).
      operationId: RestV1AssetsGet
      x-api-path-slug: restv1assets-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: with_count
      responses:
        200:
          description: OK
      tags:
      - Assets
      - (2
      - "1"
      - Only)
    post:
      summary: asset (2.1 only)
      description: Assuming that there is no "new_asset" already existing
      operationId: RestV1AssetsPost
      x-api-path-slug: restv1assets-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - (2
      - "1"
      - Only)
    patch:
      summary: assets (2.1 only)
      description: Assets (2.1 only).
      operationId: RestV1AssetsPatch
      x-api-path-slug: restv1assets-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Assets
      - (2
      - "1"
      - Only)
  /rest/v1/assets/paint/reference-files/no-locale:
    get:
      summary: asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocaleGet
      x-api-path-slug: restv1assetspaintreferencefilesnolocale-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Reference
      - File
      - (2
      - "1"
      - Only)
    post:
      summary: asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocalePost
      x-api-path-slug: restv1assetspaintreferencefilesnolocale-post
      parameters:
      - in: header
        name: Content-Type
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Reference
      - File
      - (2
      - "1"
      - Only)
  /rest/v1/assets/paint/reference-files/no-locale/download:
    get:
      summary: download asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocaleDownloadGet
      x-api-path-slug: restv1assetspaintreferencefilesnolocaledownload-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - Asset
      - Reference
      - File
      - (2
      - "1"
      - Only)
  /rest/v1/assets/paint/variation-files/ecommerce/no-locale:
    get:
      summary: asset variation file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset, an existing channel and an activated locale if the asset is localizable
        (it should be equal to "no-locale" otherwise)
      operationId: RestV1AssetsPaintVariationFilesEcommerceNoLocaleGet
      x-api-path-slug: restv1assetspaintvariationfilesecommercenolocale-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Variation
      - File
      - (2
      - "1"
      - Only)
    post:
      summary: asset variation file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset, an existing channel and an activated locale if the asset is localizable
        (it should be equal to "no-locale" otherwise)
      operationId: RestV1AssetsPaintVariationFilesEcommerceNoLocalePost
      x-api-path-slug: restv1assetspaintvariationfilesecommercenolocale-post
      parameters:
      - in: header
        name: Content-Type
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Variation
      - File
      - (2
      - "1"
      - Only)
  /rest/v1/assets/paint/variation-files/ecommerce/no-locale/download:
    get:
      summary: download asset variation file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset, an existing channel and an activated locale if the asset is localizable
        (it should be equal to "no-locale" otherwise)
      operationId: RestV1AssetsPaintVariationFilesEcommerceNoLocaleDownloadGet
      x-api-path-slug: restv1assetspaintvariationfilesecommercenolocaledownload-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - Asset
      - Variation
      - File
      - (2
      - "1"
      - Only)
  /rest/v1/asset-categories/asset_main_catalog:
    get:
      summary: asset category (2.1 only)
      description: Assuming that the given code is the code of an existing asset category
      operationId: RestV1AssetCategoriesAssetMainCatalogGet
      x-api-path-slug: restv1assetcategoriesasset-main-catalog-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Category
      - (2
      - "1"
      - Only)
  /rest/v1/asset-categories:
    get:
      summary: asset categories (2.1 only)
      description: Asset categories (2.1 only).
      operationId: RestV1AssetCategoriesGet
      x-api-path-slug: restv1assetcategories-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: with_count
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Categories
      - (2
      - "1"
      - Only)
    post:
      summary: asset category (2.1 only)
      description: Assuming that there is no "new_asset_category" already existing
      operationId: RestV1AssetCategoriesPost
      x-api-path-slug: restv1assetcategories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Category
      - (2
      - "1"
      - Only)
    patch:
      summary: asset categories (2.1 only)
      description: Asset categories (2.1 only).
      operationId: RestV1AssetCategoriesPatch
      x-api-path-slug: restv1assetcategories-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Categories
      - (2
      - "1"
      - Only)
  /rest/v1/asset-categories/new_asset_category:
    patch:
      summary: asset category (2.1 only)
      description: Asset category (2.1 only).
      operationId: RestV1AssetCategoriesNewAssetCategoryPatch
      x-api-path-slug: restv1assetcategoriesnew-asset-category-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Category
      - (2
      - "1"
      - Only)
  /rest/v1/asset-tags/colored:
    get:
      summary: asset tag (2.1 only)
      description: Assuming that the given code is the code of an existing asset tag
      operationId: RestV1AssetTagsColoredGet
      x-api-path-slug: restv1assettagscolored-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Tag
      - (2
      - "1"
      - Only)
    patch:
      summary: asset tag (2.1 only)
      description: Asset tag (2.1 only).
      operationId: RestV1AssetTagsColoredPatch
      x-api-path-slug: restv1assettagscolored-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Tag
      - (2
      - "1"
      - Only)
  /rest/v1/asset-tags:
    get:
      summary: asset tags (2.1 only)
      description: Asset tags (2.1 only).
      operationId: RestV1AssetTagsGet
      x-api-path-slug: restv1assettags-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: with_count
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Tags
      - (2
      - "1"
      - Only)
  /rest/v1/association-types/upsell:
    get:
      summary: association type (2.x only)
      description: Assuming that the given code is the code of an existing association
        type
      operationId: RestV1AssociationTypesUpsellGet
      x-api-path-slug: restv1associationtypesupsell-get
      responses:
        200:
          description: OK
      tags:
      - Association
      - Type
      - (2
      - X
      - Only)
    patch:
      summary: association type (2.x only)
      description: Association type (2.x only).
      operationId: RestV1AssociationTypesUpsellPatch
      x-api-path-slug: restv1associationtypesupsell-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Association
      - Type
      - (2
      - X
      - Only)
  /rest/v1/association-types:
    get:
      summary: association types (2.x only)
      description: Association types (2.x only).
      operationId: RestV1AssociationTypesGet
      x-api-path-slug: restv1associationtypes-get
      responses:
        200:
          description: OK
      tags:
      - Association
      - Types
      - (2
      - X
      - Only)
    post:
      summary: association type (2.x only)
      description: Assuming that there is no "new_association_type" already existing
      operationId: RestV1AssociationTypesPost
      x-api-path-slug: restv1associationtypes-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Association
      - Type
      - (2
      - X
      - Only)
    patch:
      summary: association types (2.x only)
      description: Association types (2.x only).
      operationId: RestV1AssociationTypesPatch
      x-api-path-slug: restv1associationtypes-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Association
      - Types
      - (2
      - X
      - Only)
  /rest/v1/attributes/auto_exposure:
    get:
      summary: attribute
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesAutoExposureGet
      x-api-path-slug: restv1attributesauto-exposure-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
    patch:
      summary: attribute
      description: Attribute.
      operationId: RestV1AttributesAutoExposurePatch
      x-api-path-slug: restv1attributesauto-exposure-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
  /rest/v1/attributes:
    get:
      summary: attributes
      description: Attributes.
      operationId: RestV1AttributesGet
      x-api-path-slug: restv1attributes-get
      responses:
        200:
          description: OK
      tags:
      - Attributes
    post:
      summary: attribute
      description: Assuming that there is no "new_attribute" already existing
      operationId: RestV1AttributesPost
      x-api-path-slug: restv1attributes-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
    patch:
      summary: attributes
      description: Attributes.
      operationId: RestV1AttributesPatch
      x-api-path-slug: restv1attributes-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /rest/v1/attributes/main_color/options/white:
    get:
      summary: attribute option
      description: Assuming that the given codes are respectively the code of an existing
        attribute and an existing option of this attribute
      operationId: RestV1AttributesMainColorOptionsWhiteGet
      x-api-path-slug: restv1attributesmain-coloroptionswhite-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option
    patch:
      summary: attribute option
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesMainColorOptionsWhitePatch
      x-api-path-slug: restv1attributesmain-coloroptionswhite-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option
  /rest/v1/attributes/main_color/options:
    get:
      summary: attribute options
      description: Attribute options.
      operationId: RestV1AttributesMainColorOptionsGet
      x-api-path-slug: restv1attributesmain-coloroptions-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Options
    post:
      summary: attribute option
      description: Assuming that there is no "yellow" option already existing for
        the given attribute
      operationId: RestV1AttributesMainColorOptionsPost
      x-api-path-slug: restv1attributesmain-coloroptions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option
    patch:
      summary: attribute options (2.1 only)
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesMainColorOptionsPatch
      x-api-path-slug: restv1attributesmain-coloroptions-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Options
      - (2
      - "1"
      - Only)
  /rest/v1/attribute-groups/technical:
    get:
      summary: attribute group (2.x only)
      description: Assuming that the given code is the code of an existing attribute
        group
      operationId: RestV1AttributeGroupsTechnicalGet
      x-api-path-slug: restv1attributegroupstechnical-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
    patch:
      summary: attribute group (2.x only)
      description: Attribute group (2.x only).
      operationId: RestV1AttributeGroupsTechnicalPatch
      x-api-path-slug: restv1attributegroupstechnical-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
  /rest/v1/attribute-groups:
    get:
      summary: attribute groups (2.x only)
      description: Attribute groups (2.x only).
      operationId: RestV1AttributeGroupsGet
      x-api-path-slug: restv1attributegroups-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Groups
      - (2
      - X
      - Only)
    post:
      summary: attribute group (2.x only)
      description: Assuming that there is no "new_attribute_group" already existing
      operationId: RestV1AttributeGroupsPost
      x-api-path-slug: restv1attributegroups-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
    patch:
      summary: attribute groups (2.x only)
      description: Attribute groups (2.x only).
      operationId: RestV1AttributeGroupsPatch
      x-api-path-slug: restv1attributegroups-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Groups
      - (2
      - X
      - Only)
  /rest/v1/categories/master:
    get:
      summary: category
      description: Assuming that the given code is the code of an existing category
      operationId: RestV1CategoriesMasterGet
      x-api-path-slug: restv1categoriesmaster-get
      responses:
        200:
          description: OK
      tags:
      - Category
  /rest/v1/categories:
    get:
      summary: categories
      description: Categories.
      operationId: RestV1CategoriesGet
      x-api-path-slug: restv1categories-get
      responses:
        200:
          description: OK
      tags:
      - Categories
    post:
      summary: category
      description: Assuming that there is no "new_category" already existing
      operationId: RestV1CategoriesPost
      x-api-path-slug: restv1categories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Category
    patch:
      summary: categories
      description: Categories.
      operationId: RestV1CategoriesPatch
      x-api-path-slug: restv1categories-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Categories
  /rest/v1/categories/audio_video:
    patch:
      summary: category
      description: Category.
      operationId: RestV1CategoriesAudioVideoPatch
      x-api-path-slug: restv1categoriesaudio-video-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Category
  /rest/v1/channels/ecommerce:
    get:
      summary: channel
      description: Assuming that the given code is the code of an existing channel
      operationId: RestV1ChannelsEcommerceGet
      x-api-path-slug: restv1channelsecommerce-get
      responses:
        200:
          description: OK
      tags:
      - Channel
  /rest/v1/channels:
    get:
      summary: channels
      description: Channels.
      operationId: RestV1ChannelsGet
      x-api-path-slug: restv1channels-get
      responses:
        200:
          description: OK
      tags:
      - Channels
    post:
      summary: channel (2.x only)
      description: Assuming that there is no "new_channel" already existing
      operationId: RestV1ChannelsPost
      x-api-path-slug: restv1channels-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Channel
      - (2
      - X
      - Only)
    patch:
      summary: channels (2.x only)
      description: Channels (2.x only).
      operationId: RestV1ChannelsPatch
      x-api-path-slug: restv1channels-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Channels
      - (2
      - X
      - Only)
  /rest/v1/channels/my_new_channel_3:
    patch:
      summary: channel (2.x only)
      description: Channel (2.x only).
      operationId: RestV1ChannelsMyNewChannel3Patch
      x-api-path-slug: restv1channelsmy-new-channel-3-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Channel
      - (2
      - X
      - Only)
  /rest/v1/currencies/USD:
    get:
      summary: currency (2.x only)
      description: Assuming that the given code is the code of an existing currency
      operationId: RestV1CurrenciesUSDGet
      x-api-path-slug: restv1currenciesusd-get
      responses:
        200:
          description: OK
      tags:
      - Currency
      - (2
      - X
      - Only)
  /rest/v1/currencies:
    get:
      summary: currencies (2.x only)
      description: Currencies (2.x only).
      operationId: RestV1CurrenciesGet
      x-api-path-slug: restv1currencies-get
      responses:
        200:
          description: OK
      tags:
      - Currencies
      - (2
      - X
      - Only)
  /rest/v1/families/camcorders:
    get:
      summary: family
      description: Assuming that the given code is the code of an existing family
      operationId: RestV1FamiliesCamcordersGet
      x-api-path-slug: restv1familiescamcorders-get
      responses:
        200:
          description: OK
      tags:
      - Family
    patch:
      summary: family
      description: Family.
      operationId: RestV1FamiliesCamcordersPatch
      x-api-path-slug: restv1familiescamcorders-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Family
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