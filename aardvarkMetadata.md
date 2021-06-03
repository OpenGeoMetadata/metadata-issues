This is an overview of the GeoBlacklight Metadata Elements, Version Aardvark.
## Brief


| Aardvark-id | Label                                     | URI                    | Obligation  |
|-------------|-------------------------------------------|------------------------|-------------|
| 01          | *[Title](#title)*                          | `dct_title_s`          | Required    |
| 02          | [Alternative-Title](#alternative-title)   | `dct_alternative_sm`   | Optional    |
| 03          | [Description](#description)               | `dct_description_sm`   | Recommended |
| 04          | [Language](#language)                     | `dct_language_sm`      | Optional    |
| 05          | [Creator](#creator)                       | `dct_creator_sm`       | Recommended |
| 06          | [Publisher](#publisher)                   | `dct_publisher_sm`     | Recommended |
| 07          | [Provider](#provider)                     | `schema_provider_s`    | Recommended |
| 08          | *[Resource-Class](#resource-class)*         | `gbl_resourceClass_sm` | Required    |
| 09          | [Resource-Type](#resource-type)           | `gbl_resourceType_sm`  | Recommended |
| 10          | [Subject](#subject)                       | `dct_subject_sm`       | Optional    |
| 11          | [ISO-Topic-Category](#iso-topic-category) | `dcat_theme_sm`        | Optional    |
| 12          | [Keyword](#keyword)                       | `dcat_keyword_sm`      | Optional    |
| 13          | [Temporal-Coverage](#temporal-coverage)   | `dct_temporal_sm`      | Recommended |
| 14          | [Date-Issued](#date-issued)               | `dct_issued_s`         | Optional    |
| 15          | [Index-Year](#index-year)                 | `gbl_indexYear_im`     | Recommended |
| 16          | [Date-Range](#date-range)                 | `gbl_dateRange_drsim`  | Optional    |
| 17          | [Spatial-Coverage](#spatial-coverage)     | `dct_spatial_sm`       | Recommended |
| 18          | [Spatial-Extent](#spatial-extent)         | `locn_geometry`        | Recommended |
| 19          | [Centroid](#centroid)                     | `dcat_centroid_ss`     | Optional    |
| 20          | [Relation](#relation)                     | `dct_relation_sm`      | Optional    |
| 21          | [Member-Of](#member-of)                   | `pcdm_memberOf_sm`     | Optional    |
| 22          | [Is-Part-Of](#is-part-of)                 | `dct_isPartOf_sm`      | Optional    |
| 23          | [Source](#source)                         | `dct_source_sm`        | Optional    |
| 24          | [Version](#version)                       | `dct_isVersionOf_sm`   | Optional    |
| 25          | [Replaces](#replaces)                     | `dct_replaces_sm`      | Optional    |
| 26          | [Is-Replaced-By](#is-replaced-by)         | `dct_isReplacedBy_sm`  | Optional    |
| 27          | [Rights](#rights)                         | `dct_rights_sm`        | Recommended |
| 28          | [Rights-Holder](#rights-holder)           | `dct_rightsHolder_sm`  | Optional    |
| 29          | [License](#license)                       | `dct_license_sm`       | Optional    |
| 30          | *[Access-Rights](#access-rights)*           | `dct_accessRights_s`   | Required    |
| 31          | [Format](#format)                         | `dct_format_s`         | Conditional |
| 32          | [File-Size](#file-size)                   | `gbl_fileSize_s`       | Optional    |
| 33          | [WxS-Identifier](#wxs-identifier)         | `gbl_wxsIdentifier_s`  | Conditional |
| 34          | [References](#references)                 | `dct_references_s`     | Recommended |
| 35          | *[ID](#id)*                                 | `id`                   | Required    |
| 36          | [Identifier](#identifier)                 | `dct_identifier_sm`    | Recommended |
| 37          | *[Modified](#modified)*                     | `gbl_mdModified_dt`    | Required    |
| 38          | *[Metadata-Version](#metadata-version)*     | `gbl_mdVersion_s`      | Required    |
| 39          | [Suppressed](#suppressed)                 | `gbl_suppressed_b`     | Optional    |
| 40          | [Georeferenced](#georeferenced)           | `gbl_georeferenced_b`  | Optional    |



## Title
| Label                 | Title                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:--------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aardvark-id           | 01                                                                                                                                                                                                                                                                                                                                                                                                                         |
| URI                   | `dct_title_s`                                                                                                                                                                                                                                                                                                                                                                                                              |
| Obligation            | Required                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Multiplicity          | 1-1                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Field type            | string                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Purpose               | To provide the user with the name of the resource                                                                                                                                                                                                                                                                                                                                                                          |
| Entry Guidelines      | Titles should include place names and dates when available.                                                                                                                                                                                                                                                                                                                                                                |
| Commentary            | The title is the most prominent metadata field that users see when browsing or scanning search results. Since many datasets are created with ambiguous or non-unique titles, it may be worth the effort to improve or enhance them. The ideal sequence of a title is something akin to Topic of Layer: Place, Year. Putting the year at the end of a title produces better search results, since titles are left-anchored. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Example value         | "Address Points: Ann Arbor, Michigan, 2010"                                                                                                                                                                                                                                                                                                                                                                                  |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Group                 | Bibliographic - general


## Alternative Title

| Label                 | Alternative Title                                                                                                                                                                                                                                                                                                                                                                   |
|:--------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aardvark-id           | 02                                                                                                                                                                                                                                                                                                                                                                                  |
| URI                   | `dct_alternative_sm`                                                                                                                                                                                                                                                                                                                                                                |
| Obligation            | Optional                                                                                                                                                                                                                                                                                                                                                                            |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                                                                                                                                                 |
| Field type            | string                                                                                                                                                                                                                                                                                                                                                                              |
| Purpose               | To provide the user with the another title if needed                                                                                                                                                                                                                                                                                                                                |
| Entry Guidelines      | This could be for a secondary or original title or subtitle.                                                                                                                                                                                                                                                                                                                        |
| Commentary            | For discoverability, improving titles for data is encouraged. The Alternative Title field could be a place to keep the original title. It could also be useful for scanned maps. Some have long titles that include MARC subtitle fields, such as 245$b. Whether or not Alternative Title should appear in your GeoBlacklight item view pages can be customized in the application. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                                                                                                  |
| Example value         | "NEZ H Districts"                                                                                                                                                                                                                                                                                                                                                                   |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                                                                                                |
| Group                 | Bibliographic - general

## Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

| Label                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                       |
| :---------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 03                                                                                                                                                                                                                                                                                                                                                                                                                                |
| URI                   | `dct_description_sm`                                                                                                                                                                                                                                                                                                                                                                                                              |
| Obligation            | Recommended                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Multiplicity          | 0-\*                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Field type            | string                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Purpose               | To provide the user with a summary of the resource                                                                                                                                                                                                                                                                                                                                                                                |
| Entry Guidelines      | At minimum, this is a reiteration of the title in sentence format. Other relevant information, such as data creation methods, data sources, and special licenses, may also be included. Description is a plain text field by default.                                                                                                                                                                                             |
| Commentary            | The Description field is the second most prominent value (after Title) that users see when search or browsing for items. Although not required, it is strongly recommended. If the description is minimal or lacking, it can be improved by concatenating available metadata fields, such as title, date, format, and place. This is a plain text field, so html code is not supported here unless the application is customized. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Example value         | "This polygon shapefile represents boundaries of election districts in New York City. It was harvested from the NYC Open Data Portal."                                                                                                                                                                                                                                                                                            |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Group                 | Bibliographic - general

## Language

| Label                 | Language                                                                                              |
| :---------------------|:----------------------------------------------------------------------------------------------------- |
| Aardvark-id           | 04                                                                                                    |
| URI                   | `dct_language_sm`                                                                                     |
| Obligation            | Optional                                                                                              |
| Multiplicity          | 0-\*                                                                                                  |
| Field type            | string                                                                                                |
| Purpose               | To provide the user with the language of the map                                                      |
| Entry Guidelines      | Enter a 3-letter code using the ISO 639-3 standard                                                    |
| Commentary            | This field is intended to indicate the language of the dataset, map, and/or supporting documentation. |
| Controlled Vocabulary | yes - not strict                                                                                      |
| Example value         | eng                                                                                                   |
| Element Set           | DCMI                                                                                                  |
| Group                 | Bibliographic - general                                                                               |

## Creator

| Label                 | Creator                                                                                                                                                                                                                               |
|:--------------------- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aardvark-id           | 05                                                                                                                                                                                                                                    |
| URI                   | `dct_creator_sm`                                                                                                                                                                                                                      |
| Obligation            | Recommended                                                                                                                                                                                                                           |
| Multiplicity          | 0-\*                                                                                                                                                                                                                                  |
| Field type            | string                                                                                                                                                                                                                                |
| Purpose               | To credit the person/organization that collected or authored the resource.                                                                                                                                                            |
| Entry Guidelines      | The suggested controlled vocabulary is the Library of Congress Name Authority File                                                                                                                                                    |
| Commentary            | This field is best reserved for instances in which an individual person has collected, produced, or generated analyses of data (as opposed to an agency releasing a data product or resource). It can be a person or an organization. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                    |
| Example value         | Geological Survey (U.S.)                                                                                                                                                                                                              |
| Element Set           | DCMI                                                                                                                                                                                                                                  |
| Group                 | Bibliographic - entity                                                                                                                                                                                                                |

## Publisher

| Label                 | Publisher                                                                                                                                                                                                                                  |
|:----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 06                                                                                                                                                                                                                                         |
| URI                   | `dct_publisher_sm`                                                                                                                                                                                                                           |
| Obligation            | Recommended                                                                                                                                                                                                                                |
| Multiplicity          | 0-*                                                                                                                                                                                                                                        |
| Field type            | string                                                                                                                                                                                                                                     |
| Purpose               | To credit the entity that first made a new version of something available                                                                                                                                                                  |
| Entry Guidelines      | The suggested controlled vocabulary is the Library of Congress Name Authority File                                                                                                                                                         |
| Commentary            | The distinction between dc_publisher_s and dc_creator_sm for data is often vague. Publishers should be the administrative body or organization that made the original resource available, regardless of who compiled or produced the data. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                         |
| Example value         | "ML InfoMap (Firm)"                                                                                                                                                                                                                        |
| Element Set           | DCMI                                                                                                                                                                                                                                       |
| Group                 | Bibliographic - entity                                                                                                                                                                                                                     |

## Provider

| Label                 | Provider                                                                                                                                                                                                                                                                                                                                       |
|:----------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 07                                                                                                                                                                                                                                                                                                                                             |
| URI                   | `schema_provider_s`                                                                                                                                                                                                                                                                                                                              |
| Obligation            | Recommended                                                                                                                                                                                                                                                                                                                                    |
| Multiplicity          | 1-1                                                                                                                                                                                                                                                                                                                                            |
| Field type            | string                                                                                                                                                                                                                                                                                                                                         |
| Purpose               | To clarify which organization is holds the resource or acts as the custodian for the metadata record and to help users understand which resources they can access.                                                                                                                                                                             |
| Entry Guidelines      | The value for this field is ideally be one of the names for each institution that have been coded in the GeoBlacklight application. This will embed the correct icon into the search results and item pages.                                                                                                                                   |
| Commentary            | This field previously was known as "Provenance". If the value matches one of the SVG images in the application (https://github.com/geoblacklight/geoblacklight/tree/main/app/assets/images/blacklight), it will display as an icon next to the title. GeoBlacklight organizations are encouraged to submit institutional icons to the project. |
| Controlled Vocabulary | yes - not strict                                                                                                                                                                                                                                                                                                                               |
| Example value         | University of Minnesota                                                                                                                                                                                                                                                                                                                        |
| Element Set           | schema.org                                                                                                                                                                                                                                                                                                                                     |
| Group                 | Administrative - entity                                                                                                                                                                                                                                                                                                                        |

## Resource Class

| Label                 | Resource Class                                                                                                 |
|:----------------------|:---------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 08                                                                                                             |
| URI                   | `gbl_resourceClass_sm`                                                                                           |
| Obligation            | Required                                                                                                       |
| Multiplicity          | 1-5                                                                                                            |
| Field type            | string                                                                                                         |
| Purpose               | To provide a top level set of categories for classifying the item.                                             |
| Entry Guidelines      | Choose one or more terms from the following list: Datasets, Maps, Imagery, Collections, Websites, Web services |
| Commentary            | This field is intended to help users sort between significantly different types of resources.                  |
| Controlled Vocabulary | yes - strict                                                                                                   |
| Example value         | Datasets                                                                                                       |
| Element Set           | GBL                                                                                                            |
| Group                 | Categories                                                                                                     |


## Resource Type
| Label                 | Resource Type                                                                                                                                                                                                                                                   |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 09                                                                                                                                                                                                                                                              |
| URI                   | `gbl_resourceType_sm`                                                                                                                                                                                                                                             |
| Obligation            | Recommended                                                                                                                                                                                                                                                     |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                             |
| Field type            | string                                                                                                                                                                                                                                                          |
| Purpose               | To provide a secondary level of categories for classifying the spatial type or structure of a dataset.                                                                                                                                                          |
| Entry Guidelines      | Choose one or more terms from this list.  Other terms are allowed.                                                                                                                                                                                              |
| Commentary            | This field combines an established list of terms for scanned maps (Cartographic Genres) and a custom list for geospatial data types. Additional terms are welcomed - please submit them to the community for review and inclusion into the official vocabulary. |
| Controlled Vocabulary | yes-not strict                                                                                                                                                                                                                                                  |
| Example value         | Point data                                                                                                                                                                                                                                                      |
| Element Set           | GBL                                                                                                                                                                                                                                                             |
| Group                 | Categories                                                                                                                                                                                                                                                      |


## Subject
| Label                 | Subject                                                                                                         |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 10                                                                                                              |
| URI                   | `dct_subject_sm`                                                                                                  |
| Obligation            | Optional                                                                                                        |
| Multiplicity          | 0-*                                                                                                             |
| Field type            | string                                                                                                          |
| Purpose               | To provide an all-purpose field for subjects. Any value is allowed, but controlled vocabularies are encouraged. |
| Entry Guidelines      | Any value is allowed, but controlled vocabularies are encouraged.                                               |
| Commentary            |                                                                                                                 |
| Controlled Vocabulary | no                                                                                                              |
| Example value         |                                                                                                                 |
| Element Set           | DCMI                                                                                                            |
| Group                 | Categories                                                                                                      |


## ISO Topic Category (Theme)

| Label                 | ISO Topic Category                                                                                                                                                                                                                                                |
|:-----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 11                                                                                                                                                                                                                                                                |
| URI                   | `dcat_theme_sm`                                                                                                                                                                                                                                                     |
| Obligation            | Optional                                                                                                                                                                                                                                                          |
| Multiplicity          | 0-19                                                                                                                                                                                                                                                              |
| Field type            | string                                                                                                                                                                                                                                                            |
| Purpose               | To provide a dedicated field that is restricted to ISO Topic Categories only.                                                                                                                                                                                     |
| Entry Guidelines      | Insert one or more of the ISO Topic Categories from this list                                                                                                                                                                                                     |
| Commentary            | Although ISO Topic categories are well-established and widely used, the spellings of these terms vary across domains and disciplines. The GeoBlacklight Metadata Application Profile recommends that the terms are capitalized and spaced for better readability. |
| Controlled Vocabulary | yes - strict                                                                                                                                                                                                                                                      |
| Example value         | Imagery and Base Maps                                                                                                                                                                                                                                             |
| Element Set           | DCAT                                                                                                                                                                                                                                                              |
| Group                 | Categories                                                                                                                                                                                                                                                        |


## Keyword

| Label                 | Keyword                                                                                                                                                                                                                       |
|:-----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 12                                                                                                                                                                                                                            |
| URI                   | `dcat_keyword_sm`                                                                                                                                                                                                               |
| Obligation            | Optional                                                                                                                                                                                                                      |
| Multiplicity          | 0-*                                                                                                                                                                                                                           |
| Field type            | string                                                                                                                                                                                                                        |
| Purpose               | To improve search results with hidden free text tags and to give administrators a field for internal tags                                                                                                                     |
| Entry Guidelines      | Enter tags that will be useful for enhancing searches and interpretation. Keywords will be in the metadata, but will be hidden to the user by default.                                                                        |
| Commentary            | These may be used for administrative purposes or to facilitate text seaching without cluttering a facet or interface. They may be helpful for grouping items by an accession code or for alternate spellings of common terms. |
| Controlled Vocabulary | no                                                                                                                                                                                                                            |
| Example value         | covid19                                                                                                                                                                                                                       |
| Element Set           | DCAT                                                                                                                                                                                                                          |
| Group                 | Categories                                                                                                                                                                                                                    |


## Temporal Coverage

| Label                 | Temporal Coverage                                                                                                                                                                                                                                                    |
|:-----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 13                                                                                                                                                                                                                                                                   |
| URI                   | `dct_temporal_sm`                                                                                                                                                                                                                                                      |
| Obligation            | Recommended                                                                                                                                                                                                                                                          |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                                  |
| Field type            | string                                                                                                                                                                                                                                                               |
| Purpose               | To provide the user with a free text description of the time period or ranges of what is depicted in the resource                                                                                                                                                    |
| Entry Guidelines      | This is a text string and can indicate uncertainty                                                                                                                                                                                                                   |
| Commentary            | The `dct_temporal_sm` field is multi-valued, so multiple strings can be used to indicate the time period the resource depicts, when the data was collected, and/or when the resources was created. Examples include: “approximately 1910”, “1800-1805”, “before 2000”. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                   |
| Example value         | 1980-1995                                                                                                                                                                                                                                                            |
| Element Set           | DCMI                                                                                                                                                                                                                                                                 |
| Group                 | Temporal                                                                                                                                                                                                                                                             |

## Date Issued

| Label                 | Date Issued                                                                                                                                                                                                                                                                                                           |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 14                                                                                                                                                                                                                                                                                                                    |
| URI                   | `dct_issued_s`                                                                                                                                                                                                                                                                                                          |
| Obligation            | Optional                                                                                                                                                                                                                                                                                                              |
| Multiplicity          | 0-1                                                                                                                                                                                                                                                                                                                   |
| Field type            | string                                                                                                                                                                                                                                                                                                                |
| Purpose               | To provide the user of when an item was published and for administrators to determine the age of the resource                                                                                                                                                                                                         |
| Entry Guidelines      | A single year is the preferred format. For more precide dates, use the ISO format without the time value: YYYY-MM-DD or YYYY-MM.                                                                                                                                                                                      |
| Commentary            | Although the `dct_issued_s` field is optional, it is often useful when a clear Temporal Coverage value is not present. For example, one may want to preserve a dataset with an uncertain lineage, but there is an indicator on a data portal on the date of last update. In most cases, the 4 digit year is sufficient. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                                    |
| Example value         | 1999                                                                                                                                                                                                                                                                                                                  |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                                  |
| Group                 | Temporal                                                                                                                                                                                                                                                                                                              |

## Index Year

| Label                 | Index Year                                                    |
|:-----------------------|:---------------------------------------------------------------|
| Aardvark-id           | 15                                                            |
| URI                   | `gbl_indexYear_im`                                              |
| Obligation            | Recommended                                                   |
| Multiplicity          | 1-*                                                           |
| Field type            | integer                                                       |
| Purpose               | To power time sliders widgets that rely on integers for dates |
| Entry Guidelines      | Enter one or more 4 digit integers                            |
| Commentary            |                                                               |
| Controlled Vocabulary | no                                                            |
| Example value         | 1980,1981,1982                                                |
| Element Set           | GBL                                                           |
| Group                 | Temporal                                                      |

## Date Range

| Label                 | Date Range                                                                                         |
|:-----------------------|:----------------------------------------------------------------------------------------------------|
| Aardvark-id           | 16                                                                                                 |
| URI                   | `gbl_dateRange_drsim`                                                                                |
| Obligation            | Optional                                                                                           |
| Multiplicity          | 0-*                                                                                                |
| Field type            | date-range                                                                                         |
| Purpose               | To power other time widgets that use a date range                                                  |
| Entry Guidelines      | Enter a start date and end date in the Solr daterange field convention: [YYYY to YYYY]             |
| Commentary            | This field is not yet supported by GeoBlacklight, but the application can be customized to use it. |
| Controlled Vocabulary | no                                                                                                 |
| Example value         | [1980 TO 1995]                                                                                     |
| Element Set           | GBL                                                                                                |
| Group                 | Temporal                                                                                           |


## Spatial Coverage

| Label                 | Spatial Coverage                                                                                                                                                                                       |
|:-----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 17                                                                                                                                                                                                     |
| URI                   |`dct_spatial_sm`                                                                                                                                                                                         |
| Obligation            | Recommended                                                                                                                                                                                            |
| Multiplicity          | 0-*                                                                                                                                                                                                    |
| Field type            | string                                                                                                                                                                                                 |
| Purpose               | To provide the user with a list of searchable and selectable place names                                                                                                                               |
| Entry Guidelines      | Place name text strings should be specified out to the nation level. It is typical for the place name to represent the largest extent the data layer represents. Our recommended thesaurus is GeoNames |
| Commentary            | It is recommended to have at least one place name for each layer that corresponds to the logical extent of the area of that layer.                                                                     |
| Controlled Vocabulary | yes- not strict                                                                                                                                                                                        |
| Example value         | Philadelphia, Pennsylvania, United States                                                                                                                                                              |
| Element Set           | DCMI                                                                                                                                                                                                   |
| Group                 | Spatial                                                                                                                                                                                                |

## Spatial Extent

| Label                 | Spatial Extent                                                                                                         |
|:--------------------- |:---------------------------------------------------------------------------------------------------------------------- |
| Aardvark-id           | 18                                                                                                                     |
| URI                   | `locn_geometry`                                                                                                         |
| Obligation            | Recommended                                                                                                            |
| Multiplicity          | 0-*                                                                                                                   |
| Field type            | string                                                                                                                 |
| Purpose               | To display the extent of the resource and to power the map search. This may be a bounding box or more complex geometry |
| Entry Guidelines      | For a bounding box, it should be in this format: ENVELOPE(w,e,n,s)                                                     |
| Commentary            | This field can support bounding boxes or complex geometries.                                                           |
| Controlled Vocabulary | no                                                                                                                     |
| Example value         | For bounding boxes: ENVELOPE(-97.251,-90.9229,49.3788,43.4649)<br>For geometries:                                      |
| Element Set           | LOCN/DCAT                                                                                                              |
| Group                 | Spatial                                                                                                                |

## Centroid

| Label                 | Centroid                                                                                    |
|:-----------------------|:---------------------------------------------------------------------------------------------|
| Aardvark-id           | 19                                                                                          |
| URI                   | `dcat_centroid_ss`                                                                            |
| Obligation            | Optional                                                                                    |
| Multiplicity          | 0-1                                                                                         |
| Field type            | string                                                                                      |
| Purpose               | To display the center point of a resource or otherwise a geotagged point on a map           |
| Entry Guidelines      | Enter two decimal degree coordinates separated by a comma in this order: longitude,latitude |
| Commentary            | This field is currently only supported by customizations to the GeoBlacklight application.  |
| Controlled Vocabulary | no                                                                                          |
| Example value         | 46.4218,-94.087                                                                             |
| Element Set           | DCAT                                                                                        |
| Group                 | Spatial                                                                                     |

## Relation

| Label                 | Relation                                                             |
|:-----------------------|:----------------------------------------------------------------------|
| Aardvark-id           | 20                                                                   |
| URI                   | `dct_relation_sm`                                                      |
| Obligation            | Optional                                                             |
| Multiplicity          | 0-*                                                                  |
| Field type            | string                                                               |
| Purpose               | To link items with a general, unspecified relationship to each other |
| Entry Guidelines      | Enter only the ID of the related item(s)                             |
| Commentary            |                                                                      |
| Controlled Vocabulary | no                                                                   |
| Example value         |                                                                      |
| Element Set           | DCMI                                                                 |
| Group                 | Relations                                                            |

## Member Of

| Label                 | Member Of                                                                                        |
|:-----------------------|:--------------------------------------------------------------------------------------------------|
| Aardvark-id           | 21                                                                                               |
| URI                   | `pcdm_memberOf_sm`                                                                                 |
| Obligation            | Optional                                                                                         |
| Multiplicity          | 0-*                                                                                              |
| Field type            | string                                                                                           |
| Purpose               | To link items that are part of a collection                                                      |
| Entry Guidelines      | Make a collection record to group records together. Enter the ID of the Collection level record. |
| Commentary            |                                                                                                  |
| Controlled Vocabulary | no                                                                                               |
| Example value         |                                                                                                  |
| Element Set           | PCDM                                                                                             |
| Group                 | Relations                                                                                        |

## Is Part Of

| Label                 | Is Part Of                                                                                        |
| :--------------------- | :------------------------------------------------------------------------------------------------- |
| Aardvark-id           | 22                                                                                                |
| URI                   | `dct_isPartOf_sm`                                                                                 |
| Obligation            | Optional                                                                                          |
| Multiplicity          | 0-\*                                                                                              |
| Field type            | string                                                                                            |
| Purpose               | To link items that are a subset of another item (ex. page in a book)                              |
| Entry Guidelines      | <br><br>Make a parent record to group records together. Enter the ID of the parent record(s).<br> |
| Commentary            |                                                                                                   |
| Controlled Vocabulary | no                                                                                                |
| Example value         |                                                                                                   |
| Element Set           | DCMI                                                                                              |
| Group                 | Relations                                                                                         |


## Source

| Label                 | Source                                                                                               |
|:-----------------------|:------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 23                                                                                                   |
| URI                   | `dct_source_sm`                                                                                        |
| Obligation            | Optional                                                                                             |
| Multiplicity          | 0-*                                                                                                  |
| Field type            | string                                                                                               |
| Purpose               | To link items that have been derived from another item (ex. digitized shapefile from historical map) |
| Entry Guidelines      | Enter the ID of the item(s) that the resource was derived from                                       |
| Commentary            |                                                                                                      |
| Controlled Vocabulary | no                                                                                                   |
| Example value         |                                                                                                      |
| Element Set           | DCMI                                                                                                 |
| Group                 |                                                                                                      |


## Is Version Of

| Label                 | Version                                                                                                                                        |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 24                                                                                                                                             |
| URI                   | `dct_isVersionOf_sm`                                                                                                                             |
| Obligation            | Optional                                                                                                                                       |
| Multiplicity          | 0-*                                                                                                                                            |
| Field type            | string                                                                                                                                         |
| Purpose               | To indicate that an item is part of a series of resources that are updated or altered and to provide a link to a different variant or adaption |
| Entry Guidelines      | Enter the ID of the most recent related record OR create a parent record to group versions together.                                           |
| Commentary            |                                                                                                                                                |
| Controlled Vocabulary | no                                                                                                                                             |
| Example value         |                                                                                                                                                |
| Element Set           | DCMI                                                                                                                                           |
| Group                 | Relations                                                                                                                                      |


## Replaces

| Label                 | Replaces                                                                                                                                                                                                                                                                                                        |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 25                                                                                                                                                                                                                                                                                                              |
| URI                   | `dct_replaces_sm`                                                                                                                                                                                                                                                                                                 |
| Obligation            | Optional                                                                                                                                                                                                                                                                                                        |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                                                                             |
| Field type            | string                                                                                                                                                                                                                                                                                                          |
| Purpose               | To point user to deprecated item                                                                                                                                                                                                                                                                                |
| Entry Guidelines      | Enter the ID of the deprecated related item(s)                                                                                                                                                                                                                                                                  |
| Commentary            | Replaces and Is Replaced By can be used for a revised version of a research dataset where the original is needed for reference. For example, if the original dataset has already been cited somewhere, it can be retained in a repository with a clear indication that it has been superceded by a new version. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                              |
| Example value         |                                                                                                                                                                                                                                                                                                                 |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                            |
| Group                 | Relations                                                                                                                                                                                                                                                                                                       |


#Is Replaced By

| Label                 | Is Replaced By                                                                                                                                                                                                                                                                                                  |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 26                                                                                                                                                                                                                                                                                                              |
| URI                   | `dct_isReplacedBy_sm`                                                                                                                                                                                                                                                                                             |
| Obligation            | Optional                                                                                                                                                                                                                                                                                                        |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                                                                             |
| Field type            | string                                                                                                                                                                                                                                                                                                          |
| Purpose               | To point user to new item                                                                                                                                                                                                                                                                                       |
| Entry Guidelines      | Enter the ID of the related item(s) that should be used instead.                                                                                                                                                                                                                                                |
| Commentary            | Replaces and Is Replaced By can be used for a revised version of a research dataset where the original is needed for reference. For example, if the original dataset has already been cited somewhere, it can be retained in a repository with a clear indication that it has been superceded by a new version. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                              |
| Example value         |                                                                                                                                                                                                                                                                                                                 |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                            |
| Group                 | Relations                                                                                                                                                                                                                                                                                                       |


## Rights

| Label                 | Rights                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|:----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 27                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| URI                   | `dct_rights_sm`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Obligation            | Recommended                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Field type            | string                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Purpose               | To provide a free text field for rights information, such as usage, access, or copyright                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Entry Guidelines      | Enter free text of generic, catch-all access and usage rights. It can include clickable links; all access and usage rights.                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Commentary            | This field is intended to be flexible to accommodate different types of rights and disclaimers. Users are encouraged to adopt one of the rightsstatements.org statements.                                                                                                                                                                                                                                                                                                                                                                                 |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Example value         | All data is copyrighted by China Data Center and/or its suppliers. Derived works that include the source data must be merged with other value-added data in such a way that the derived work cannot be converted back to the original source data format. This data is licensed by UC Berkeley for research, educational, and other non-commercial use by authorized users, which include persons affiliated with UC Berkeley and walk-in users who must access the data in person at the library. https://rightsstatements.org/page/InC/1.0/?language=en |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Group                 | Rights                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |


## Rights Holder

| Label                 | Rights Holder                                                                                                                                                                                                              |
|:-----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 28                                                                                                                                                                                                                         |
| URI                   | `dct_rightsHolder_sm`                                                                                                                                                                                                        |
| Obligation            | Optional                                                                                                                                                                                                                   |
| Multiplicity          | 0-*                                                                                                                                                                                                                        |
| Field type            | string                                                                                                                                                                                                                     |
| Purpose               | To clarify which person or organization owns or controls the rights for this version of the item                                                                                                                           |
| Entry Guidelines      | Enter the name of the person or organization. If applicable, the suggested controlled vocabulary is the Library of Congress Name Authority File                                                                            |
| Commentary            | This can be used for instances in which an an organization owns a digital copy of an analog resource or otherwise controls access. This is different that Provider, which refers more to the resource or metadata steward. |
| Controlled Vocabulary | no                                                                                                                                                                                                                         |
| Example value         | Johns Hopkins University Libraries                                                                                                                                                                                         |
| Element Set           | DCMI                                                                                                                                                                                                                       |
| Group                 | Rights                                                                                                                                                                                                                     |


## License

| Label                 | License                                                                                                                                     |
|:-----------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 29                                                                                                                                          |
| URI                   | `dct_license_sm`                                                                                                                              |
| Obligation            | Optional                                                                                                                                    |
| Multiplicity          | 0-*                                                                                                                                         |
| Field type            | string                                                                                                                                      |
| Purpose               | To provide URI links to specific, known licenses                                                                                            |
| Entry Guidelines      | Enter only a URI. Recommended sources are https://creativecommons.org or https://opendatacommons.org/                                       |
| Commentary            | This field is only for URIs of known licenses. Do not enter a rightsstatement.org statement here, because those belong in the Rights field. |
| Controlled Vocabulary | no                                                                                                                                          |
| Example value         | https://creativecommons.org/licenses/by/4.0/                                                                                                |
| Element Set           | DCMI                                                                                                                                        |
| Group                 | Rights                                                                                                                                      |


## Access Rights

| Label                 | Access Rights                                                                                                                                                                                                                                    |
|:-----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 30                                                                                                                                                                                                                                               |
| URI                   | `dct_accessRights_s`                                                                                                                                                                                                                               |
| Obligation            | Required                                                                                                                                                                                                                                         |
| Multiplicity          | 1-1                                                                                                                                                                                                                                              |
| Field type            | string                                                                                                                                                                                                                                           |
| Purpose               | To clarify to the user if the resource is public (any user can access) or restricted (a user will need to log in to some kind of authentication protocol) and if the application should provide a web service preview and/or a download function |
| Entry Guidelines      | Only one of two values are allowed: Public or Restricted                                                                                                                                                                                         |
| Commentary            | This field can be set to "Public", which allows users to view and download an item, or "Restricted", which requires a user to log in to an authentication service.                                                                               |
| Controlled Vocabulary | yes - strict                                                                                                                                                                                                                                     |
| Example value         | Public                                                                                                                                                                                                                                           |
| Element Set           | DCMI                                                                                                                                                                                                                                             |
| Group                 | Rights                                                                                                                                                                                                                                           |


## Format

| Label                 | Format                                                                                                                                                                                                                                                                                        |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 31                                                                                                                                                                                                                                                                                            |
| URI                   | `dct_format_s`                                                                                                                                                                                                                                                                                  |
| Obligation            | Conditional                                                                                                                                                                                                                                                                                   |
| Multiplicity          | 0-1 or 1-1                                                                                                                                                                                                                                                                                    |
| Field type            | string                                                                                                                                                                                                                                                                                        |
| Purpose               | To display to the user the name of the file type as a text string in the Download button                                                                                                                                                                                                      |
| Entry Guidelines      | if download URL is configured as a single key:value pair                                                                                                                                                                                                                                      |
| Commentary            | A long list of formats is available here. The most important thing to remember about the dc_format_s field is that it is required for Download functionality if using a single value string for downloads. (pre-GeoBlacklight version 3.0). See the Multiple Downloads guide for more details |
| Controlled Vocabulary | yes-not strict                                                                                                                                                                                                                                                                                |
| Example value         | Shapefile                                                                                                                                                                                                                                                                                     |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                          |
| Group                 | Distribution                                                                                                                                                                                                                                                                                  |


## File Size

| Label                 | File Size                                                                                                                                                   |
|:-----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 32                                                                                                                                                          |
| URI                   | `gbl_fileSize_s`                                                                                                                                              |
| Obligation            | Optional                                                                                                                                                    |
| Multiplicity          | 0-1                                                                                                                                                         |
| Field type            | string                                                                                                                                                      |
| Purpose               | To inform the user of the size of the file download                                                                                                         |
| Entry Guidelines      | Enter the size in megabytes                                                                                                                                 |
| Commentary            | This field is intended to give users a sense of how large the data or image they are interested in downloading, and serves to alert users about huge files. |
| Controlled Vocabulary | no                                                                                                                                                          |
| Example value         | 25.96 MB                                                                                                                                                    |
| Element Set           | GBL                                                                                                                                                         |
| Group                 | Distribution                                                                                                                                                |


## WxS Identifier
| Label                 | WxS Identifier                                                                                                                                                        |
|:----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 33                                                                                                                                                                    |
| URI                   | `gbl_wxsIdentifier_s`                                                                                                                                                   |
| Obligation            | Conditional                                                                                                                                                           |
| Multiplicity          | 0-1 or 1-1                                                                                                                                                            |
| Field type            | string                                                                                                                                                                |
| Purpose               | To identify the layer or store for a WFS, WMS, or WCS web service so the application can construct the full web service link                                          |
| Entry Guidelines      | Only the layer name is added here. The base service endpoint URLs (e.g. "https://maps-public.geo.nyu.edu/geoserver/sdr/wms") are added to the dct_references_s field. |
| Commentary            | The WxS Indentifer is used to point to specific layers within an OGC geospatial web service. This field is not used for ArcGIS Rest Services.                         |
| Controlled Vocabulary | no                                                                                                                                                                    |
| Example value         | druid:vr593vj7147                                                                                                                                                     |
| Element Set           | GBL                                                                                                                                                                   |
| Group                 | Distribution                                                                                                                                                          |


## References

| Label                 | References                                                                                                                                                                                                                       |
|:-----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 34                                                                                                                                                                                                                               |
| URI                   | `dct_references_s`                                                                                                                                                                                                                 |
| Obligation            | Recommended                                                                                                                                                                                                                      |
| Multiplicity          | 0-1                                                                                                                                                                                                                              |
| Field type            | string JSON                                                                                                                                                                                                                      |
| Purpose               | To provide external URLs for accessing or describing the resource                                                                                                                                                                |
| Entry Guidelines      | The field dct_references_s defines external services and references using the CatInterOp approach. The field value is a serialized JSON array of key/value pairs, with keys representing XML namespace URI's and values the URL. |
| Commentary            | All of the external links for the resource are added to the dct_references_s field as a serialized JSON array of key/value pairs. The download key/value pair is unique, because the value can be an array.                      |
| Controlled Vocabulary | no                                                                                                                                                                                                                               |
| Example value         | "dct_references_s": "{\"http://schema.org/url\":\"http://purl.stanford.edu/bm662dm5913\",\"http://schema.org/downloadUrl\":\"http://stacks.stanford.edu/file/druid:bm662dm5913/data.zip\"}"                                      |
| Element Set           | DCMI                                                                                                                                                                                                                             |
| Group                 | Distribution                                                                                                                                                                                                                     |


## ID

| Label                 | ID                                                                                                                                                                                                           |
|:-----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 35                                                                                                                                                                                                           |
| URI                   | `id`                                                                                                                                                                                                           |
| Obligation            | Required                                                                                                                                                                                                     |
| Multiplicity          | 1-1                                                                                                                                                                                                          |
| Field type            | string                                                                                                                                                                                                       |
| Purpose               | To provide a unique alpha-numberic ID for the item that will act as the primary key in Solr and to create a unique landing page for the item                                                                 |
| Entry Guidelines      | This string must be a globally unique value. The value should be alpha-numeric characters separated by dashes.                                                                                               |
| Commentary            | The ID makes up the URL for the resource in GeoBlacklight. If having a readable slug is desired, it is common to use the form, institution-keyword1-keyword2 (words or characters are separated by hyphens). |
| Controlled Vocabulary | no                                                                                                                                                                                                           |
| Example value         | princeton-rv042w38t                                                                                                                                                                                          |
| Element Set           | GBL                                                                                                                                                                                                          |
| Group                 | Administrative                                                                                                                                                                                               |


## Identifier

| Label                 | Identifier                                                                                                                                                                                                                                                                                                                                                                                               |
|:-----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 36                                                                                                                                                                                                                                                                                                                                                                                                       |
| URI                   | `dct_identifier_sm`                                                                                                                                                                                                                                                                                                                                                                                        |
| Obligation            | Recommended                                                                                                                                                                                                                                                                                                                                                                                              |
| Multiplicity          | 0-*                                                                                                                                                                                                                                                                                                                                                                                                      |
| Field type            | string                                                                                                                                                                                                                                                                                                                                                                                                   |
| Purpose               | To provide a general purpose field for identifiers                                                                                                                                                                                                                                                                                                                                                       |
| Entry Guidelines      | This may include a DOI, catalog number, and/or other system number                                                                                                                                                                                                                                                                                                                                       |
| Commentary            | This field is not displayed in the interface. At least one value would ideally a persistent identifier or permalink (such as a [PURL (https://en.wikipedia.org/wiki/Persistent_uniform_resource_locator) or Handle (https://en.wikipedia.org/wiki/Handle_System). Additional values can be for other identifiers used by the resource, such as the call number, OCLC number, or other system identifier. |
| Controlled Vocabulary | no                                                                                                                                                                                                                                                                                                                                                                                                       |
| Example value         | 5864 .L7 E635 1998 .G7                                                                                                                                                                                                                                                                                                                                                                                   |
| Element Set           | DCMI                                                                                                                                                                                                                                                                                                                                                                                                     |
| Group                 | Administrative                                                                                                                                                                                                                                                                                                                                                                                           |


## Modified

| Label                 | Modified                                                                                  |
|:-----------------------|:-------------------------------------------------------------------------------------------|
| Aardvark-id           | 37                                                                                        |
| URI                   | `gbl_mdModified_dt`                                                                         |
| Obligation            | Required                                                                                  |
| Multiplicity          | 0-1                                                                                       |
| Field type            | date-time                                                                                 |
| Purpose               | To inform administrators of when the metadata was last touched                            |
| Entry Guidelines      | Use the XML Schema dateTime format (YYYY-MM-DDThh:mm:ssZ)                                 |
| Commentary            | This value should indicate when the metadata (not the resource itself) was last modified. |
| Controlled Vocabulary | no                                                                                        |
| Example value         | 2015-01-01T12:00:00Z                                                                      |
| Element Set           | GBL                                                                                       |
| Group                 | Administrative                                                                            |


## Metadata Version

| Label                 | Metadata Version                                                                 |
|:-----------------------|:----------------------------------------------------------------------------------|
| Aardvark-id           | 38                                                                               |
| URI                   | `gbl_mdVersion_s`                                                                  |
| Obligation            | Required                                                                         |
| Multiplicity          | 1-1                                                                              |
| Field type            | string                                                                           |
| Purpose               | To clarify which GeoBlacklight metadata schema is being used                     |
| Entry Guidelines      | Enter the string: Aardvark                                                       |
| Commentary            | There have been two metadata schema versions for GeoBlacklight: 1.0 and Aardvark |
| Controlled Vocabulary | yes -strict                                                                      |
| Example value         | Aardvark                                                                         |
| Element Set           | GBL                                                                              |
| Group                 | Administrative                                                                   |


## Suppressed

| Label                 | Suppressed                                                                                                                                                                              |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 39                                                                                                                                                                                      |
| URI                   | `gbl_suppressed_b`                                                                                                                                                                        |
| Obligation            | Optional                                                                                                                                                                                |
| Multiplicity          | 0-1                                                                                                                                                                                     |
| Field type            | string boolean                                                                                                                                                                          |
| Purpose               | To hide items from users in the search results. If set to True, the record will not appear in search results. It is still accessible from the Data Relations widget and via direct URL. |
| Entry Guidelines      | Only one of two values are allowed: true or false                                                                                                                                       |
| Commentary            | This field is useful for multipart items with identical metadata, such as pages in an atlas or series.                                                                                  |
| Controlled Vocabulary | yes -strict                                                                                                                                                                             |
| Example value         | true                                                                                                                                                                                    |
| Element Set           | GBL                                                                                                                                                                                     |
| Group                 | Administrative                                                                                                                                                                          |


## Georeferenced

| Label                 | Georeferenced                                                                                                                                                                                                       |
|:-----------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aardvark-id           | 40                                                                                                                                                                                                                  |
| URI                   | `gbl_georeferenced_b`                                                                                                                                                                                                 |
| Obligation            | Optional                                                                                                                                                                                                            |
| Multiplicity          | 0-1                                                                                                                                                                                                                 |
| Field type            | string boolean                                                                                                                                                                                                      |
| Purpose               | To indicate whether or not a scanned map or other imagery has a georeferenced version                                                                                                                               |
| Entry Guidelines      | Only one of two values are allowed: true or false                                                                                                                                                                   |
| Commentary            | This field can be a shortcut for users to find georeferenced maps. Administrators can also employ the Source field to link a paper map with its scane (e.g. a TIFF) and its georeferenced version (e.g. a GEOTIFF.) |
| Controlled Vocabulary | yes -strict                                                                                                                                                                                                         |
| Example value         | false                                                                                                                                                                                                               |
| Element Set           | GBL                                                                                                                                                                                                                 |
| Group                 | Administrative                                                                                                                                                                                                      |



