# ![LOGO](logo.png) BC Laws **flow**ground Connector

## Description

A generated **flow**ground connector for the BC Laws API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/bclaws.ca/bclaws/1.0.0/openapi.json<br/>
Generated at: 2019-05-07T17:39:36+03:00

## API Description

BC Laws is an electronic library providing free public access to the laws of British Columbia. BC Laws is hosted by the Queen's Printer of British Columbia and published in partnership with the Ministry of Justice and the Law Clerk of the Legislative Assembly.BC Laws contains a comprehensive collection of BC legislation and related materials. It is available on the internet in two forms:First: The library is available as a web site in which users can browse and search the laws of British Columbia.Second: The library is available as a portal to legislation in raw XML data format, accessible via the BC Laws API2. This direct access to raw data is intended to enable third parties to build or add their own custom applications based on the structure of the data and all the associated search functionality inherent in that structure. The BC Laws website itself is an example of one such application. 

Please note that you may experience issues when submitting requests to the delivery or test environment if using this [OpenAPI specification](https://github.com/bcgov/api-specs) in other API console viewers.

## Authorization

This API does not require authorization.

## Actions

### Describes the documents and directories available within a specific 'aspect' (content group) of the BCLaws library

*Tags:* `content`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.

### Lists the metadata available for the specified index or directory from the BCLaws legislative respository

*Tags:* `content`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.
* `civixDocumentId` - _required_ - The document identification code for an index or directory

### Retrieves a specific document from the BCLaws legislative repository (HTML format)

> The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.

*Tags:* `document`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.
* `civixIndexId` - _required_ - Index identification code
* `civixDocumentId` - _required_ - The document identification code for an index or directory

### Retrieves a specific document from the BCLaws legislative repository with search text highlighted (HTML format)

> The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.

*Tags:* `document`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.
* `civixIndexId` - _required_ - Index identification code
* `civixDocumentId` - _required_ - The document identification code for an index or directory
* `searchString` - _required_ - The text to search for within the document

### Retrieves a specific document from the BCLaws legislative repository (XML format)

> The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.

*Tags:* `document`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.
* `civixIndexId` - _required_ - Index identification code
* `civixDocumentId` - _required_ - The document identification code for an index or directory

### Retrieves a specific document from the BCLaws legislative repository with search text highlighted (XML format)

> The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.

*Tags:* `document`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.
* `civixIndexId` - _required_ - Index identification code
* `civixDocumentId` - _required_ - The document identification code for an index or directory
* `searchString` - _required_ - The text to search for within the document

### A listing of metadata available for the specified aspect and search term from the BCLaws legislative repository

*Tags:* `search`

#### Input Parameters
* `aspectId` - _required_ - The identifier of the 'aspect' (content group) to search
    Possible values: complete, corpreg, bcgaz1, bcgaz2, oic, psl, ecb, hscr, arch_oic.
* `q` - _required_ - query term
* `s` - _required_ - first hit (start index)
* `e` - _required_ - last hit (end index)
* `nFrag` - _required_ - number of fragment snippets to return (< 10)
* `lFrag` - _required_ - length of fragment snippets (< 200)

## License

**flow**ground :- Telekom iPaaS / bclaws-ca-bclaws-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
