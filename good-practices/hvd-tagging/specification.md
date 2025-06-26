
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

This good practice candidate is based on the exchanges, proposals and decisions from the participants in the ISO & GeoDCAT-AP Metadata Implementation Pilot to develop an agreed way to tag geospatial / INSPIRE High-Value Datasets (HVD), with the purpose of duly identifying amd transforming their corresponding dataset metadata descriptions from the ISO 19115 format (highly used by the INSPIRE Community) into the geospatial extension of the DCAT-AP format used by the Open Data community (GeoDCAT-AP). 

-- ADD MORE CONTEXT ON GREENDATA4ALL, ETC.

This document leverages on the initial discussions collected and described in the [Repository for Action 2.5 of the INSPIRE MIWP on the alignment of High-value datasets and INSPIRE](https://github.com/INSPIRE-MIF/hvd-inspire), made by members of the INSPIRE community.

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
