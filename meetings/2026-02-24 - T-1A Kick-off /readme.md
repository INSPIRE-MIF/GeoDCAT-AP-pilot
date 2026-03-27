# Pilot Phase 2 - Working Team T-1A Kick-off meeting (24 February 2026)

## Agenda

* Welcome
* Pilot Phase 2 Working Teams - Objectives & Set up (JRC) -  10 minutes
* Latest GeoDCAT-AP release - v3.1.0 (SEMIC) - 10 minutes
* Repositories for sharing and discussing issues - Procedure Remainder (JRC & SEMIC) - 5 minutes
* ISO-GeoDCAT-AP Issues - Guided Discussion (JRC & SEMIC & All) - max. 90 minutes
* Summary of actions from the meeting (JRC) - 5 minutes
* AoB (All)

## Participants

* Member States: Belgium (BE-Flanders), Denmark (DK), Italy (IT), Latvia (LV), Malta (MT), Finland (FI), Germany (DE), the Netherlands (NL), Spain (ES).
* European Commission: Directorate-General for Environment (ENV), Publications Office of the European Union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General Joint Research Centre (JRC), the European Environment Agency (EEA).
* Contractors: con terra, Epsilon Italia.

## Presentations and recording

Presentations can be downloaded [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2026-02-24%20-%20T-1A%20Kick-off%20/presentations).

Recording: Available on request. 

## Meeting summary

The objectives of the meeting were:
* Explaining the purpose of Phase 2 and why specialised working groups are needed.
    * Generally define the scope, expected deliverables and timelines for each working team (T-1A, T-1B, T-2).
    * Clarify the working plan (independent work with regular cross‑team coordination) and potential interactions between them.
* Presenting the key changes introduced in GeoDCAT-AP version 3.1.0.
* Identifying the procedure and the GitHub repositories that will be used during Phase 2 of the pilot for raising, gathering community inputs and reaching agreements.
* Reviewing the most critical open issues and refresh the community about them.
    * Gathering community feedback on existing proposals.
    * Highlighting the importance of community participation on GitHub to identify common solutions and reach future consensus.
* Recap any important decisions taken and trace specific actions for future working team meetings.

The JRC opened the meeting, welcoming the participants and confirming the agenda. 

###  Pilot Phase 2 Working Teams – Objectives & Set up
The JRC delivered a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-24%20-%20T-1A%20Kick-off%20/presentations/20260224_01_ISO%26GeoDCAT-AP_Pilot_Ph%202-T1-A_Kick_off-JRC.pptx) explaining the purpose of Phase 2 and, more concretely, the different specialised working teams created. These will operate independently but in a coordinated manner:
*	T-1A (the one kicked-off in this meeting). Working team focused on managing issues with an impact on geospatial metadata harvesting and reporting of geospatial High-Value Datasets (HVDs), scoped in the integration of INSPIRE geospatial assets into data.europa.eu (hence, highly related to the ISO-to-GeoDCAT-AP mapping and transformation).
*	T-1B. Working team focused on specific analysis and good practices for the alignment of INSPIRE into data.europa.eu which deserve special attention and/or require substantial effort - mainly highlighting:
    *	Formalisation of the geospatial HVD tagging good practice.
    *	Agreement on a good practice for the description of data service / APIs, and related mapping and transformation issues.
    *	Analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation.
    *	Identification of any remaining gaps and discussion on the need for tackling them.
*	T-2. Working team focused on explore the use of Artificial Intelligence (AI) assisted tools in metadata generation, and other potential uses in metadata management tasks.

The initial plan is to organise working team meetings monthly, supported by continuous coordination, and bi-monthly / quarterly general pilot meetings to exchange progress and updates.

### Latest GeoDCAT AP release – v3.1.0

SEMIC described the main changes from [version 3.0.0](https://semiceu.github.io/GeoDCAT-AP/releases/3.0.0/) and provided the link to the [version 3.1.0 changelog](https://semiceu.github.io/GeoDCAT-AP/releases/3.1.0/CHANGELOG.html), which summarises all the release artefacts.

Additionally, the changes which may affect the current work of the working teams were highlighted, especially the mapping of distributions and handling of geospatial HVDs. 

### Repositories for sharing and discussing issues - Procedure Remainder

SEMIC and the JRC reminded about the intended use of the pilot repositories - In summary, using:
* the SEMIC repositories: [for GeoDCAT-AP specification issues](https://github.com/SEMICeu/GeoDCAT-AP/issues) / [for GeoDCAT-AP XSLT transformations issues](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues).
* the ISO & GeoDCAT-AP pilot repository: only [for discussing issues concerned to the management of the pilot](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues)

The JRC emphasised that the Excel summary spreadsheet from pìlot Phase 1 will not be longer maintained. All activity, discussions and agreements will be tracked directly on the above-entioned GitHub repositories.

### ISO-GeoDCAT-AP Issues - Guided Discussion

The JRC provided a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-24%20-%20T-1A%20Kick-off%20/presentations/20260224_03_ISO%26GeoDCAT-AP_Pilot_Ph%202-T1-A_ISO-GeoDCAT-AP%20Issues-JRC.pptx) summarising the most burning issues in the context of the ISO-to-GeoDCAT-AP mapping and transformation.

* Most critical issues / Prioritised issues
    * Distributions and their mapping in GeoDCAT-AP
        * Main issue: [Geo-DCAT-AP #139](https://github.com/SEMICeu/GeoDCAT-AP/issues/139) - Mapping for Resource locator (On-line resource)
        * Related ones: [Pilot #9](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/9); [XSLT #57](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/57); [Geo-DCAT-AP #135](https://github.com/SEMICeu/GeoDCAT-AP/issues/135); [XSLT #74](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/74); [XSLT #98](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/98); [Pilot #8](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/8); 

    * Identification of HVDs
        * [Pilot #3](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/3) / [GeoDCAT-AP #147](https://github.com/SEMICeu/GeoDCAT-AP/issues/147) / [Pilot #7](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/7) - The three issues related to the implementation of the geospatial HVD tagging good practice, are now implemented in the SEMIC XSLT.
        * [Pilot #2](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/2) - proposals related to the HVD-tagging good practice and the XSL transformation, now clarified with the implementation of the good practice in the SEMIC XSLT.
        * [GeoDCAT-AP #134](https://github.com/SEMICeu/GeoDCAT-AP/issues/134) - Lack of information retrieval when having to process Anchor encodings.

* Less prioritised issues:
    * [GeoDCAT-AP #140](https://github.com/SEMICeu/GeoDCAT-AP/issues/140) - Coupled resource
    * [XSLT #78](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/78) - Identifiers in ISO metadata / parentIdentifier not mapped to DCAT-AP or GeoDCAT-AP

* ISSUES NOT DISCUSSED:
    * [XSLT #84](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/84) - Support for gmd:status
    * [XSLT #64](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/64) - Multiple geometry serialisations for dcat:bbox
    * [Pilot #11](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/11) - Issues transforming service and multilingual metadata
    * [XSLT #71](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/71) - Support for more than one dataset identifier
    * [XSLT #72](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/72) - Duplicity of schema:startDate/schema:endDate after transformation
    * [GeoDCAT-AP #171](https://github.com/SEMICeu/GeoDCAT-AP/issues/171) - OGC EPSG Coordinate Reference Systems Register too narrow?

## Agreements / Actions

- [ ] **Action 1**. The INSPIRE commmunity is requested to revise the list of open issues above and provide relevant feedback. This is especially needed for the issues concerned to 'Distributions and their mapping in GeoDCAT-AP' - i.e.,:
    - Main issue: [Geo-DCAT-AP #139](https://github.com/SEMICeu/GeoDCAT-AP/issues/139) - Mapping for Resource locator (On-line resource)
    - Related ones: [Pilot #9](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/9); [XSLT #57](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/57); [Geo-DCAT-AP #135](https://github.com/SEMICeu/GeoDCAT-AP/issues/135); [XSLT #74](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/74); [XSLT #98](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/98); [Pilot #8](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/8);  
- [x] **Action 2**. Close the following issues: [Pilot #3](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/3) / [Pilot #7](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/7) / [Pilot #2](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/2)
- [x] **Action 3**. Open a new issue thread to discuss 'how to refer in the future to other legislations different from theELI-codes of High Value Dataset/ODD legislation, such as the ones from the PriorityDatasets codelist, in GeoDCAT-AP'. This topic was pending from [Pilot #2](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/2), which is now closed.
    - The new issue is already open and available: [SEMICeu/GeoDCAT-AP#173](https://github.com/SEMICeu/GeoDCAT-AP/issues/173)
- [x] **Action 4**. Regarding [GeoDCAT-AP #147](https://github.com/SEMICeu/GeoDCAT-AP/issues/147), it was raised the need to analyse how to help users to understand the information across the different SEMIC standards and navigate through them easily. The idea is to enhance the documentation to help the users. 
 need to analyse how to help users to understand the information across the different standards and navigate through them easily (enhance the documentation).
- [x] **Action 5**. Regarding [GeoDCAT-AP #134](https://github.com/SEMICeu/GeoDCAT-AP/issues/134), keep it open asking the community if something else in the thread needs to be revisited now that the geospatial HVD tagging good practice has been agreed and implemented in the SEMIC XSLT.
- [x] **Action 6**. Regarding [GeoDCAT-AP #140](https://github.com/SEMICeu/GeoDCAT-AP/issues/140), it was decided to add to GeoDCAT-AP section 'A.7.6 Coupled resource' a note (and an XML example) explaining that INSPIRE allows a more simple implementation of the Coupled Resource linkage (e.g. a URI pointing to the dataset or dataset series metadata record, instead to pointing to the dataset or dataset series).
- [x] **Action 7**. Regarding [XSLT #78](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/78) and the mapping of the parentIdentifier ISO metadata field, it was decided to consider the mapping proposed by the work in the ISO TC211 internal draft of ISO/TS 19115-5, which defines the mapping of ISO metadata to DCAT at global (international) level. In that mapping, the parentIdentifier field is mapped to dcat:inSeries.
- [ ] **Action 8**. For the agenda of the next T-1A working team meeting, continue the dicussion on open issue (with special focus on the ones regarded to 'Distributions and their mapping in GeoDCAT-AP'), as well as the list of 'ISSUES NOT DISCUSSED' in this meeting.
