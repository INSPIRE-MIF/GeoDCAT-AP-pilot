
# Geospatial High-Value Datasets (HVDs) tagging: Good Practice guidelines

`Version: 1.0`
`Date: 2026-06-29`
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
    * [7.2. Requirements for HVD tagging](#tagging-requirements)
* [Annex A: Examples](#annex-a)


## 1. Introduction <a name="introduction"></a>

This good practice specification is based on the exchanges, proposals and agreements from the participants in the [ISO & GeoDCAT-AP Metadata Implementation Pilot](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main) to develop an agreed way to tag geospatial / INSPIRE High-Value Datasets (HVD), with the purpose of duly identifying and transforming their corresponding dataset metadata descriptions from the [ISO 19115](https://www.iso.org/standard/26020.html) format (highly used by the INSPIRE Community) into the geospatial extension of the DCAT-AP format used by the Open Data community, [GeoDCAT-AP](https://semiceu.github.io/GeoDCAT-AP/releases/3.1.0/).

The ongoing modernisation and simplification the INSPIRE Directive by aligning its provisions to the new EU digital and data horizontal legislative framework is aimed at ensuring legal coherence, reducing duplication of efforts and unnecessary burden on Member States, while preserving the Directive’s objectives of ensuring the availability, accessibility, interoperability and quality of environmental geospatial data in the Member States. This approach is in line with the [European Data Union Strategy](https://eur-lex.europa.eu/legal-content/En/TXT/?uri=COM:2025:835:FIN) and its precursor, the [European Strategy for Data](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A52020DC0066), which have the objective to build a unified European data market, fuel the development and use of Artificial Intelligence (AI), and establish the EU as a competitive, sovereign leader in the global digital economy, by scaling Up access to data, provide regulatory simplification and legal certainty and protecting digital sovereignty.

The above-mentioned horizontal EU legislation includes the [Directive (EU) 2019/1024 - Open Data Directive](http://data.europa.eu/eli/dir/2019/1024/oj) and its [Implementing Regulation (EU) 2023/138 - High-Value Datasets](https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj/eng), the [Regulation (EU) 2022/868 - Data Governance Act](https://eur-lex.europa.eu/eli/reg/2022/868/oj), and the [Regulation (EU) 2024/903 - Interoperable Europe Act](http://data.europa.eu/eli/reg/2024/903/oj), all having significant impact on the access to, reuse, interoperability, and governance of public sector data in a coherent, technologically advanced and at scale manner.

In addition, the EU’s objective of creating Common European Data Spaces set out in the European Strategy for Data, includes a dedicated Green Deal Data Space to support the European Green Deal. This requires breaking data silos and ensuring that all relevant environmental data – spatial and non-spatial – can flow freely to inform EU environmental and climate objectives and reduce administrative burden on companies and public administrations. 

Within this context, the [GreenData4All](https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/13170-GreenData4All-updated-rules-on-geospatial-environmental-data-and-access-to-environmental-information_en) initiative is triggering a deep revamp of INSPIRE with a view to supporting the transition to a greener and carbon-neutral economy, and reducing administrative burden through regulatory simplification, while taking advantage of the most updated technological trends and innovation opportunities. 

This simplification, conveyed by the [environmental simplification package](https://knowledge-base.inspire.ec.europa.eu/news-and-publications/news/simplification-inspire-directive-2025-12-10_en), will be supported by non-legislative actions and practical tools to support smart and efficient reuse of environmental data across the Union. 

It will be also ensured that INSPIRE geospatial and environmental data are made available as open data according Directive (EU) 2019/1024, using common standards, APIs, and open licenses, and maximizing accessibility and re-use for all users through the European Data Portal ([data.europa.eu](https://data.europa.eu/en)), as single entry point for European public sector data. To avoid duplication of efforts and reducing burdens for data providers, as of 1 July 2026, the [INSPIRE Geoportal](https://inspire-geoportal.ec.europa.eu/) will be discontinued and its content will be fully integrated with [data.europa.eu](https://data.europa.eu/en), operated by the [Publications Office of the European Union](https://op.europa.eu/).

In light of the above, this document addresses the need to ensure the encoding of HVD tags in geospatial dataset metadata descriptions in accordance with the applicable standards ensuring their proper accessibility and filtering in the European Data Portal.

It leverages on the initial discussions collected and described in the [Repository for Action 2.5 of the INSPIRE MIWP on the alignment of High-value datasets and INSPIRE](https://github.com/INSPIRE-MIF/hvd-inspire), made by members of the INSPIRE community.

The main reference for this specification is the [INSPIRE MD TG].

## 2. Scope <a name="scope"></a>

This document provides a set of rules, that normative and 'de facto' geospatial metadata standards can currently support, based on the list of Requirements and s agreed within the context of the [ISO & GeoDCAT-AP Metadata Implementation Pilot](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main) to appropiately tag geospatial / INSPIRE HVDs, defining concrete encoding rules.

## 3. Conformance <a name="conformance"></a>

The requirements classes expressed here apply to geospatial dataset metadata record documents.
In particular, the dataset metadata records reported by Member States in the scope of the [INSPIRE Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A02007L0002-20241126), shall be INSPIRE-compliant (verifiable through tests performed through the national instances of the Reference Validator), and should be available in the relevant national geoportal catalog (see https://knowledge-base.inspire.ec.europa.eu/tools/inspire-your-country_en) for their direct or indirect harvesting by the [European Data Portal](https://data.europa.eu/en).

## 4. Normative references <a name="normative-references"></a>

- **[ISO 19115:2005]** - EN ISO 19115:2005, *Geographic information — Metadata*
- **[ISO 19119:2016]** - EN ISO 19119:2016, *Geographic information — Services*
- **[ISO/TS 19139:2007]** - ISO/TS 19139:2007, *Geographic information — Metadata — XML schema implementation*
- **[INSPIRE MD TG]** - JRC. *Technical Guidance for the implementation of INSPIRE dataset and service metadata based on ISO/TS 19139:2007*.  v2.0.1 - 2017-03-02
- **[DCAT-AP]** - SEMIC, v.3.0 - 2024-06-14
- **[DCAT-AP HVD]** - SEMIC, *Usage guidelines of DCAT-AP for High-Value Datasets*. v. 3.0.0-hvd - 2024-10-25
- **[GeoDCAT-AP]** - SEMIC, v.3.1.0 - 2026-02-16

<!-- Second parts of the reference-style links, see also https://www.markdownguide.org/basic-syntax/#reference-style-links  -->
[ISO 19115:2005]: https://www.isotc211.org/2005/gmd "ISO 19115:2005, Geographic information — Metadata"
[ISO 19119:2016]: https://www.iso.org/standard/59221.html?browse=tc "ISO 19119:2016, Geographic information — Services"
[ISO/TS 19139:2007]: https://www.isotc211.org/2005/gmd/ "ISO/TS 19139:2007, Geographic information — Metadata — XML schema implementation"
[INSPIRE MD TG]: https://inspire.ec.europa.eu/id/document/tg/metadata-iso19139 "Technical Guidance for the implementation of INSPIRE dataset and service metadata based on ISO/TS 19139:2007"
[DCAT-AP]: https://semiceu.github.io/DCAT-AP/releases/3.0.0/
[DCAT-AP HVD]: https://semiceu.github.io/DCAT-AP/releases/3.0.0-hvd/
[GeoDCAT-AP]: https://semiceu.github.io/GeoDCAT-AP/releases/3.1.0/

## 5. Terms and definitions <a name="terms-and-definitions"></a>

For the purposes of this document, the following terms and definitions apply:

| Term | Definition | Source |
| --- | --- | --- |
| dataset | Identifiable collection of data. | [ISO 19115](https://www.iso.org/obp/ui/#iso:std:iso:19115:-2:ed-2:v1:en:sec:3.6) |
| encoding | Conversion of data into a series of codes. | [ISO 19118](https://www.iso.org/obp/ui/#iso:std:iso:19118:ed-2:v1:en:term:4.13) |
| encoding rule | Identifiable collection of conversion rules that define the encoding for a particular data structure. | [ISO 19118](https://www.iso.org/obp/ui/#iso:std:iso:19118:ed-2:v1:en:term:4.14) |
| HVD (high-value datasets) | Documents the re-use of which is associated with important benefits for society, the environment and the economy, in particular because of their suitability for the creation of value-added services, applications and new, high-quality and decent jobs, and of the number of potential beneficiaries of the value-added services and applications based on those datasets | [Directive (EU) 2019/1024](http://data.europa.eu/eli/dir/2019/1024/oj) |
| HVD category | One of the thematic data categories laid down in the Annex I to Directive (EU) 2019/1024 (Open Data Directive)  | - |
| HVD subcategory | One of the high-value dataset, belonging to a HVD category, established in the Annex to the Commission Implementing Regulation (EU) 2023/138 (HVD Implementing Regulation)  | - |
| metadata | Information about a resource. | [ISO 19115](https://www.iso.org/obp/ui#iso:std:iso:19115:-1:ed-1:v1:en) |
| resource | Identifiable asset or means that fulfils a requirement (Example: dataset, dataset series, service, document, initiative, software, person or organization). | [ISO 19115](https://www.iso.org/obp/ui#iso:std:iso:19115:-1:ed-1:v1:en) |

**NOTE** ISO and the European Commission maintain comprehensive terminological databases made available at the following addresses:
- [ISO Online browsing platform](https://www.iso.org/obp)
- [INSPIRE glossary](http://inspire.ec.europa.eu/glossary)

## 6. Acronyms <a name="acronyms"></a>

| Abbreviation | Term |
| --- | --- |
| API | Application Programming Interface |
| DCAT-AP | DCAT - Application Profile |
| HVD | High-Value Dataset |
| URL | Uniform Resource Locator |


## 7. Geospatial High-Value Dataset Tagging <a name="geo-hvd-tagging"></a>

### 7.1. Main principles <a name="main-principles"></a>

[PENDING TO REVISE]
Annex I of Directive (EU) 2019/1024 lays down the list of thematic categories of high-value datasets, currently corresponding to the following data categories: 1) geospatial; 2) earth observation and environment; 3) meteorological; 4) statistics; 5) companies and company ownership; and 6) mobility. Six of them are in in the scope of the INSPIRE Directive (namely: 1) geospatial; 2) earth observation and environment; and 6) mobility).

For each of these HVD categories, Commission Implementing Regulation (EU) 2023/138 establishes the list of high-value datasets held by public sector bodies among the existing 'documents' to which that Open Data Directive applies, while also lays down the arrangements for the publication and re-use of high-value datasets. In particular, the applicable conditions for re-use (including licensing conditions) and the minimum requirements for disseminating data via Application Programming Interfaces (‘APIs’).

One of the arrangements for publication, article 3(5), states that public sector bodies holding high-value datasets shall '**ensure that the datasets are denoted as high-value datasets in their metadata description**'.

As HVDs are a subset of all datasets published as Open Data (to which the DCAT-AP metadata profile applies on general-purpose portals), [specific usage guidelines of DCAT-AP (DCAT-AP HVD)](https://semiceu.github.io/DCAT-AP/releases/2.2.0-hvd/) have been adopted to satisfy the HVD Implementing Regulation and the minimum specific metadata requirements.

This document provides with the encoding rules for tagging the geospatial datasets as high-value datasets in the ISO 19115 metadata records in order to meet the above requirement. This will enable the transformation into GeoDCAT-AP by applying the XLST script in order to make those datasets discoverable in the EU Open Data portal data.europa.eu. It, however, does not mean a complete compliance with the Regulation and the DCAT-AP HVD because not all metadata requirements in DCAT-AP HVD are covered. 

The scope of this specification is focused on defining the keywords to be used in ISO / INSPIRE metadata records, including their encoding rules, to allow machines and users to identify if a a dataset is classified as a HVD, meaning that:
- the dataset falls under the HVD Implementing Regulation;
- the dataset belongs to a HVD category and/or subcategory as set out in the Annex to the Implementing Regulation and in the [controlled vocabulary](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category) derived from it.
All other aspects (e.g. issues related to formats, data services, ...) to be taken into account to guarantee the conformance to the DCAT-AP HVD are out of the scope and are addressed in other documents [NOTE: add link].

### 7.2. Requirements for HVD tagging - Requirements class <a name="tagging-requirements"></a>

| Requirements class | http://inspire.ec.europa.eu/id/spec/ds-geospatial-hvd-tagging/1.0/ds-md-hvd-tagging |
| --- | --- |
| Target type | ISO/TS 19139:2007 Geographic information Metadata XML schema implementation (Data sets and Data set series metadata) |
| Dependency | https://inspire.ec.europa.eu/id/ats/metadata/2.0/datasets-and-series (See NOTE below) |

\* NOTE: This is the URI of the candidate Conformance Class, to be considered in a new version of the [INSPIRE MD TG] [Chapter 3.1](https://github.com/INSPIRE-MIF/technical-guidelines/blob/2022.2/metadata/metadata-iso19139/metadata-iso19139.adoc#31-baseline-metadata-for-data-sets-and-data-set-series).

Conformance to the requirement class defined in this section is verified if a geospatial dataset metadata record complies with the set of requiments defined in sections [7.2.1](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/good-practices/hvd-tagging/specification.md#721-applicable-legislation-). and [7.2.2](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/good-practices/hvd-tagging/specification.md#722-hvd-category-and-subcategory-).

### 7.2.1. Applicable legislation <a name="applicable-legislation"></a>

#### Applicable legislation and HVD keyword: Requirement `hvd-tag-req_01` and Recommendation `hvd-tag-rec_01`: 

| **Requirement `hvd-tag-req_01`** | **/req/applicable-legislation** |
| --- | --- |
| A | To declare that the dataset corresponds to one of the high-value datasets listed in the Annex of the HVD Implementing Regulation (Implementing Regulation (EU) 2023/138), and thus belonging to one of the thematic categories set out in Annex I to Directive (EU) 2019/1024,  the `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword/gmx:Anchor` element SHALL be used. |
| B | For this purpose, the `xlink:href` attribute in the `gmx:Anchor` element SHALL point to the ELI [http://data.europa.eu/eli/reg_impl/2023/138/oj](http://data.europa.eu/eli/reg_impl/2023/138/oj). |

| **Recommendation `hvd-tag-rec_01`** | **/rec/applicable-legislation-keyword** |
| --- | --- |
| A |  The keyword value encoded within the `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword/gmx:Anchor` referenced in `hvd-tag-req_01` SHOULD be the text "High-value dataset" or "HVD", in English language. |

**NOTE**: The `gmd:descriptiveKeywords` element used for the declaration of the applicable legislation shall be different from that one used for the declaration of HVD category and/or subcategory.

##### Examples of XML encoding

```xml
   <gmd:descriptiveKeywords>
		<gmd:MD_Keywords>
			<!-- HVD Keyword -->
			<gmd:keyword>
				<gmx:Anchor xlink:href="http://data.europa.eu/eli/reg_impl/2023/138/oj">High-value dataset</gmx:Anchor>
			</gmd:keyword>
		</gmd:MD_Keywords>
	</gmd:descriptiveKeywords>
```

```xml
   <gmd:descriptiveKeywords>
		<gmd:MD_Keywords>
			<!-- HVD Keyword -->
			<gmd:keyword>
				<gmx:Anchor xlink:href="http://data.europa.eu/eli/reg_impl/2023/138/oj">HVD</gmx:Anchor>
			</gmd:keyword>
		</gmd:MD_Keywords>
	</gmd:descriptiveKeywords>
```

### 7.2.2. HVD category and subcategory <a name="hvd-category"></a>

#### 7.2.2.1. HVD category / subcategory - General: 
Requirement `hvd-tag-req_02` and Recommendation `hvd-tag-rec_02`.

| **Requirement `hvd-tag-req_02`** | **/req/hvd-category-subcategory-general** |
| --- | --- |
| A | At least one HVD category or one HVD subcategory SHALL be provided as a keyword derived from the [EU Vocabularies HVD Categories]([https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category](https://op.europa.eu/en/web/eu-vocabularies/concept-scheme/-/resource?uri=http://data.europa.eu/bna/asd487ae75). | 

| **Recommendation `hvd-tag-rec_02`** | **/rec/hvd-category-subcategory-general** |
| --- | --- |
| A |  If a HVD category is provided, then the declaration of the HVD subcategory corresponding to that category is OPTIONAL and MAY be provided. And vice versa, If a HVD subcategory is provided, then the declaration of the HVD category corresponding to that subcategory is OPTIONAL and MAY be provided. |

#### 7.2.2.2. HVD category: 
Requirement `hvd-tag-req_03` and Recommendation `hvd-tag-rec_03`.

| **Requirement `hvd-tag-req_03`** | **/req/hvd-category** |
| --- | --- |
| A | If the HVD category to which the dataset belongs to is provided, it SHALL be declared using a keyword from the [EU Vocabularies HVD Categories](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category), thus corresponding to one of the HVD categories set out in the Annex to the HVD Implementing Regulation (Implementing Regulation (EU) 2023/138). | 
| B | This keyword SHALL be encoded using a `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword/gmx:Anchor` element, different from that one used for the declaration of the applicable legislation as per `hvd-tag-req_01`. |
| C | For this purpose, the `xlink:href` attribute in the `gmx:Anchor` element SHALL point to the URI corresponding to the relevant HVD category in the [EU Vocabularies HVD Categories](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category). |

| **Recommendation `hvd-tag-rec_03`** | **/rec/hvd-category** |
| --- | --- |
| A |  The keyword value encoded within the `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword/gmx:Anchor` referenced in `hvd-tag-req_03` SHOULD be the exact text value of the HVD category extracted from the [EU Vocabularies HVD Categories](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category) in the main language of the metadata record. |

##### Example of XML encoding

```xml
<!-- metadata language -->
[...]
<gmd:language>
      <gmd:LanguageCode codeList="http://www.loc.gov/standards/iso639-2" codeListValue="ita">ita</gmd:LanguageCode>
</gmd:language>
 [...]
   <gmd:descriptiveKeywords>
		<gmd:MD_Keywords>
			<!-- Category Keyword -->
			<gmd:keyword>
				<gmx:Anchor xlink:href="http://data.europa.eu/bna/c_dd313021">Dati relativi all'osservazione della terra e all'ambiente</gmx:Anchor>
			</gmd:keyword>
			[...]
		</gmd:MD_Keywords>
	</gmd:descriptiveKeywords>
```

#### 7.2.2.3. HVD subcategory: 
Requirement `hvd-tag-req_04` and Recommendation `hvd-tag-rec_04`.

| **Requirement `hvd-tag-req_04`** | **/req/hvd-subcategory** |
| --- | --- |
| A | If the HVD subcategory to which the dataset belongs to is provided, it SHALL be declared using a subcategory keyword from the [EU Vocabularies HVD Categories](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category), thus corresponding to one of the HVD subcategories set out in the Annex to the HVD Implementing Regulation (Implementing Regulation (EU) 2023/138). | 
| B | This keyword SHALL be encoded using a `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword/gmx:Anchor` element, different from that one used for the declaration of the applicable legislation as per `hvd-tag-req_01`. |
| C | For this purpose, the `xlink:href` attribute in the `gmx:Anchor` element SHALL point to the URI corresponding to the relevant HVD subcategory in the [EU Vocabularies HVD Categories](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category). |

| **Recommendation `hvd-tag-rec_04`** | **/rec/hvd-subcategory** |
| --- | --- |
| A |  The keyword value encoded within the `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:keyword/gmx:Anchor` referenced in `hvd-tag-req_04` SHOULD be the exact text value of the HVD subcategory extracted from the [EU Vocabularies HVD Categories](https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/high-value-dataset-category) in the main language of the metadata record. |

##### Example of XML encoding

```xml
<!-- metadata language -->
[...]
<gmd:language>
      <gmd:LanguageCode codeList="http://www.loc.gov/standards/iso639-2" codeListValue="ita">ita</gmd:LanguageCode>
</gmd:language>
 [...]
<gmd:descriptiveKeywords>
		<gmd:MD_Keywords>
			[...]
			<!-- Subcategory Keyword-->
			<gmd:keyword>
				<gmx:Anchor xlink:href="http://data.europa.eu/bna/c_f399050e">Regioni marine</gmx:Anchor>
			</gmd:keyword>
			[...]
		</gmd:MD_Keywords>
	</gmd:descriptiveKeywords>
```

#### 7.2.2.4. HVD categories and subcategories - Thesaurus: 
Requirement `hvd-tag-req_05` and Recommendation `hvd-tag-rec_05`.

| **Requirement `hvd-tag-req_05`** | **/req/hvd-category-subcategory-thesaurus** |
| --- | --- |
| A | When the declaration of the HVD category or subcategory is provided using a `gmd:descriptiveKeywords` element, the originating controlled vocabulary (i.e. the EU Vocabularies HVD Categories) SHALL be cited using its `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:thesaurusName/gmd:CI_Citation` element. | 
| B | The title of the vocabulary SHALL be provided using the `gmd:title/gmx:Anchor` of the above-mentioned `gmd:CI_Citation` element, where the `xlink:href` attribute SHALL contain the URI [http://data.europa.eu/bna/asd487ae75](http://data.europa.eu/bna/asd487ae75) (i.e. URI of the EU Vocabularies HVD Categories thesaurus). |
| C | The date of the vocabulary SHALL be provided using the `gmd:date/gmd:CI_Date/gmd:date/gco:Date` of the above-mentioned `gmd:CI_Citation` element. |
| NOTE | See Recommendation `hvd-tag-rec_05` for further details on the provision of the name, date and date type of the above-mentioned thesaurus. |

| **Recommendation `hvd-tag-rec_05`** | **/rec/hvd-category-subcategory-thesaurus** |
| --- | --- |
| A |  The name value encoded within the `gmd:descriptiveKeywords/gmd:MD_Keywords/gmd:thesaurusName/gmd:CI_Citation/gmd:title/gmx:Anchor` referenced in `hvd-tag-req_05` SHOULD be the text "High-value dataset categories", in English language. |
| B | The date type code of the vocabulary date referenced in `hvd-tag-req_05` SHOULD be of type `publication`, according the the [ISO 19139] CI_DateTypeCode code list. |
| NOTE | At the date of the agreements of this specification, it was recommended to use `2023-09-27` as date of publication of the EU Vocabularies HVD Categories thesaurus v1.0. |

* NOTE: Two new versions of the EU Vocabularies HVD Categories thesaurus (different from v1.0) have been published from since: v2.0 and v2.1. To be discussed with the INSPIRE Community if a  publication date different to `2023-09-27` (corresponding to v1.0) SHOULD be recommended. The example below shall be updated, if this would be the case.

##### Example of XML encoding

```xml
   <gmd:descriptiveKeywords>
		[...]
			<!-- Thesaurus Reference -->
			<gmd:thesaurusName>
				<gmd:CI_Citation>
					<gmd:title>
						<gmx:Anchor xlink:href="http://data.europa.eu/bna/asd487ae75">High-value dataset categories</gmx:Anchor>
					</gmd:title>
					<gmd:date>
						<gmd:CI_Date>
							<gmd:date>
								<gco:Date>2023-09-27</gco:Date>
							</gmd:date>
							<gmd:dateType>
								<gmd:CI_DateTypeCode codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/Codelist/ML_gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication"/>
							</gmd:dateType>
						</gmd:CI_Date>
					</gmd:date>
				</gmd:CI_Citation>
			</gmd:thesaurusName>
		</gmd:MD_Keywords>
	</gmd:descriptiveKeywords>
```

##### Complete example of XML encoding for HVD category and subcategory

```xml
<!-- metadata language -->
[...]
<gmd:language>
      <gmd:LanguageCode codeList="http://www.loc.gov/standards/iso639-2" codeListValue="eng"/>
</gmd:language>
 [...]
   <gmd:descriptiveKeywords>
		<gmd:MD_Keywords>
			<!-- Category Keyword -->
			<gmd:keyword>
				<gmx:Anchor xlink:href="http://data.europa.eu/bna/c_dd313021">Earth observation and environment</gmx:Anchor>
			</gmd:keyword>
			<!-- Subcategory Keyword-->
			<gmd:keyword>
				<gmx:Anchor xlink:href="http://data.europa.eu/bna/c_f399050e">Sea regions</gmx:Anchor>
			</gmd:keyword>
			<!-- Thesaurus Reference -->
			<gmd:thesaurusName>
				<gmd:CI_Citation>
					<gmd:title>
						<gmx:Anchor xlink:href="http://data.europa.eu/bna/asd487ae75">High-value dataset categories</gmx:Anchor>
					</gmd:title>
					<gmd:date>
						<gmd:CI_Date>
							<gmd:date>
								<gco:Date>2023-09-27</gco:Date>
							</gmd:date>
							<gmd:dateType>
								<gmd:CI_DateTypeCode codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/Codelist/ML_gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication"/>
							</gmd:dateType>
						</gmd:CI_Date>
					</gmd:date>
				</gmd:CI_Citation>
			</gmd:thesaurusName>
		</gmd:MD_Keywords>
	</gmd:descriptiveKeywords>
```

# Annex A: Examples <a name="annex-a"></a>

## Examples (XML encoded)

A complete and detailed example is available both in [multilingual version](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/good-practices/hvd-tagging/ISO_HVD_Tagging_Anchor_Multilingual-clarification.xml) and in [non-multilingual version](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/good-practices/hvd-tagging/ISO_HVD_Tagging_Anchor_Non-Multilingual-clarification.xml).

In addition, a collection of XML dataset metadata records following this good practice in Member States are available in the [implementation-examples folder](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/good-practices/hvd-tagging/implementation-examples) of the pilot repository on GitHub.

_These examples are purely informative and do not constitute a reference definition of a conformant metadata._ 



