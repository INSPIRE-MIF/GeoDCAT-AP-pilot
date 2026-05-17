
# Geospatial High-Value Datasets (HVDs) tagging: Good Practice guidelines

`Version: 1.0`
`Date: 2025-06-26`
`Note: This specification is a DRAFT - Work in progress`

## Table of Contents

* [1. Introduction](#introduction)
* [2. Scope](#scope)
* [3. Conformance](#conformance)
* [4. Normative references](#normative-references)
* [5. Terms and definitions](#terms-and-definitions)
* [6. Acronyms](#acronyms)
* [7. Geospatial High-Value Dataset Tagging](#geo-hvd-tagging)
    * [7.1. Main principles](#main-principles)
    * [7.2. Resources](#resources)
    * [7.3. Requirement classes](#reqclass)
* [Annex A: Examples](#annex-a)


## 1. Introduction <a name="introduction"></a>

This good practice candidate is based on the exchanges, proposals and decisions from the participants in the ISO & GeoDCAT-AP Metadata Implementation Pilot to develop an agreed way to tag geospatial / INSPIRE High-Value Datasets (HVD), with the purpose of duly identifying and transforming their corresponding dataset metadata descriptions from the ISO 19115 format (highly used by the INSPIRE Community) into the geospatial extension of the DCAT-AP format used by the Open Data community (GeoDCAT-AP).

The recent proposal to modernise and simplify the INSPIRE Directive by aligning its obligations with more recent horizontal EU datal legislation is aimed at ensuring legal coherence, reducing duplication and burden on Member States, while preserving the Directive’s objectives of ensuring the accessibility, quality and interoperability of environmental spatial data. This approach is in line with the [2020 European strategy for data](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A52020DC0066) initiative, which has the objective to modernise the INSPIRE Directive in line with technological developments and innovation opportunities, with a view to supporting the transition to a greener and carbon-neutral economy, and reducing administrative burden.

Horizontal EU data legislation (i.e. [Directive (EU) 2019/1024 - Open Data Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex:52023DC0703) and [Implementing Regulation (EU) 2023/138 - High-Value Datasets](https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj/eng), [Regulation (EU) 2022/868 - Data Governance Act](https://eur-lex.europa.eu/eli/reg/2022/868/oj), and [Regulation (EU) 2024/903 - Interoperable Europe Act](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R0903)) regulates the access to, reuse, interoperability, and governance of public sector data in a coherent and technologically advanced manner.

In addition, the EU’s objective of creating Common European Data Spaces set out in the 2020 European strategy for data, includes a dedicated Green Deal Data Space to support the European Green Deal; this requires breaking data silos and ensuring that all relevant environmental data – spatial and non-spatial – can flow freely to inform EU environmental and climate objectives and reduce administrative burden on companies and public administrations. 

The proposed simplification of the INSPIRE Directive, as part of the environmental simplification omnibus, constitutes the legal component of the GreenData4All initiative. It will be supported by non-legislative actions and practical tools to support smart and efficient reuse of environmental data across the Union. 

It will be also ensured that geospatial and environmental data are made available as open data, using common standards, APIs, and open licenses, thus minimizing duplication, reducing burdens for data providers, and maximizing accessibility and re-use for all users through the EU’s open data portal [data.europa.eu](https://data.europa.eu/en), which serves as the central point of access for European public data, as it is therefore also proposed to delete the obligation on the Commission to operate the Inspire geo-portal.

In light of the above, this document addresses the need to ensure to encode the dataset metadata descriptions in accordance with the standards used on the European Open Data Portal.

It leverages on the initial discussions collected and described in the [Repository for Action 2.5 of the INSPIRE MIWP on the alignment of High-value datasets and INSPIRE](https://github.com/INSPIRE-MIF/hvd-inspire), made by members of the INSPIRE community.

The main reference for the metadata specification re-used in this proposal is the [INSPIRE MD TG].

## 2. Scope <a name="scope"></a>

This document provides a set of rules, that de facto geospatial metadata standards can currently support, based on the list of Requirements and Recommendations agreed within the context of the mentioned pilot to appropiately tag geospatial / INSPIRE HVDs, defining concrete encoding rules.

## 3. Conformance <a name="conformance"></a>

The requirements classes expressed here apply to geospatial dataset metadata record documents.
In particular, the dataset metadata records reported by Member States in the scope of the INSPIRE Directive (REF), shall be INSPIRE-compliant (verifiable through tests performed in the Reference Validator), and should be available in the relevant national geoportal catalog (see https://knowledge-base.inspire.ec.europa.eu/tools/inspire-your-country_en), and consequently harvested by the [INSPIRE Geoportal](https://inspire-geoportal.ec.europa.eu).

Furthermore, at the time of writing, the requirements expressed here for the Download Services are not applicable for specifications based on OGC APIs due to the lack of an agreed mapping for some conditional and mandatory INSPIRE metadata elements (in particular the Coupled Resource, and Unique Resource Identifier) in the [OAPIF GP] document.

## 4. Normative references <a name="normative-references"></a>

- **[ISO 19115:2005]** - EN ISO 19115:2005, *Geographic information — Metadata*
- **[ISO 19119:2016]** - EN ISO 19119:2016, *Geographic information — Services*
- **[ISO/TS 19139:2007]** - ISO/TS 19139:2007, *Geographic information — Metadata — XML schema implementation*
-- CHECK LATEST VERSION
- **[INSPIRE MD TG]** - JRC. *Technical Guidance for the implementation of INSPIRE dataset and service metadata based on ISO/TS 19139:2007*.  v2.0.1 - 2017-03-02
-- ADD DCAT 3
-- Add DCAT-AP for HVDs
-- ADD GeoDCAT-AP 3
-- ADD INSPIRE Directive

<!-- Second parts of the reference-style links, see also https://www.markdownguide.org/basic-syntax/#reference-style-links  -->
[ISO 19115:2005]: https://www.isotc211.org/2005/gmd "ISO 19115:2005, Geographic information — Metadata"
[ISO 19119:2016]: https://www.iso.org/standard/59221.html?browse=tc "ISO 19119:2016, Geographic information — Services"
[ISO/TS 19139:2007]: https://www.isotc211.org/2005/gmd/ "ISO/TS 19139:2007, Geographic information — Metadata — XML schema implementation"
[INSPIRE MD TG]: https://inspire.ec.europa.eu/id/document/tg/metadata-iso19139 "Technical Guidance for the implementation of INSPIRE dataset and service metadata based on ISO/TS 19139:2007"
-- ADD OTHER THE NECESSARY LINKS

## 5. Terms and definitions <a name="terms-and-definitions"></a>

For the purposes of this document, the following terms and definitions apply:

-- ADD OTHER NECESSARY TEMRS: e.g. metadata
-- CHECK THE LINKS
| Term | Definition | Source |
| --- | --- | --- |
| dataset | Identifiable collection of data. | [ISO 19115](https://www.iso.org/obp/ui/#iso:std:iso:19115:-2:ed-2:v1:en:sec:3.6) |
| encoding | Conversion of data into a series of codes. | [ISO 19118](https://www.iso.org/obp/ui/#iso:std:iso:19118:ed-2:v1:en:term:4.13) |
| encoding rule | Identifiable collection of conversion rules that define the encoding for a particular data structure. | [ISO 19118](https://www.iso.org/obp/ui/#iso:std:iso:19118:ed-2:v1:en:term:4.14) |
| metadata | Information about a resource. | [ISO 19115](https://www.iso.org/obp/ui#iso:std:iso:19115:-1:ed-1:v1:en) |
| resource | Identifiable asset or means that fulfils a requirement (Example: dataset, dataset series, service, document, initiative, software, person or organization). | [ISO 19115](https://www.iso.org/obp/ui#iso:std:iso:19115:-1:ed-1:v1:en) |

**NOTE** ISO and the European Commission maintain comprehensive terminological databases made available at the following addresses:
- [ISO Online browsing platform](https://www.iso.org/obp)
- [INSPIRE glossary](http://inspire.ec.europa.eu/glossary)

## 6. Acronyms <a name="acronyms"></a>

| Abbreviation | Term |
| --- | --- |
| API | Application Programming Interface |
| HVD | High-Value Dataset |
| URL | Uniform Resource Locator |


## 7. Geospatial High-Value Dataset Tagging <a name="geo-hvd-tagging"></a>

<!--
--REVISE[
### 7.1. Main principles <a name="main-principles"></a>

- An INSPIRE data set shall have INSPIRE View and Download services.
- The linkage between the data set and the View and Download services shall be ensured by the bidirectional relationship between the data set metadata and the service metadata.

### 7.2. Resources <a name="resources"></a>

![Diagram of Simplified linkage model](./graphics/INSPIRE_models_v1.5_1.jpg)

![Diagram of Simplified linkage model - Mandatory linkage in the simplification approach](./graphics/INSPIRE_models_v1.5_2.jpg)

]REVISE--
--->


# Annex A: Examples <a name="annex-a"></a>

## Examples (XML encoded)
This annex points to a collection of XML dataset metadata records following this good practice.
_These examples are purely informative and do not constitute a reference definition of a conformant metadata._

The examples are available in the [implementation-examples folder](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/good-practices/hvd-tagging/implementation-examples) of the pilot repository on GitHub.
