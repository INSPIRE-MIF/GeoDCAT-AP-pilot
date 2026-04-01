# Pilot Phase 2 - Working Team T-1B Kick-off meeting (26 February 2026)

## Agenda

*	Welcome
*	Pilot Phase 2 Working Teams - Objectives & Set up (JRC) - 10 minutes
*	T-1B Objectives & Tasks 
    *	Agreement on a good practice for describing Data Services / APIs (FI & DK & JRC) - 15 minutes
        * Discussion (All) - 15 minutes
    *	Analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation (ES & JRC) - 15 minutes
        *	Discussion (All) - 15 minutes
    *	Drafting of the Geospatial High-Value Datasets tagging good practice specification (IT & JRC) - 15 minutes
        * Discussion (All) - 15 minutes
*	Summary of actions from the meeting (JRC) - 10 minutes
*	AoB (All)

## Participants

* Member States: Belgium (BE-Flanders), Croatia (HR), Denmark (DK), Italy (IT), Finland (FI), France (FR), Germany (DE), Malta (MT), the Netherlands (NL), Spain (ES).
* European Commission: Publications Office of the European Union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General Joint Research Centre (JRC), the European Environment Agency (EEA).
* Contractors: con terra, Epsilon Italia.

## Presentations and recording

Presentations can be downloaded [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-26%20-%20T-1B%20Kick-off/presentations/readme.md).

Recording: Available on request. 

## Meeting summary

The objectives of the meeting were:
* Explaining the purpose of Phase 2 and why specialised working groups are needed.
    * Generally define the scope, expected deliverables and timelines for each working team (T-1A, T-1B, T-2).
    * Clarify the working plan (independent work with regular cross‑team coordination) and potential interactions between them.
* Describe the tasks assigned to working team T-1B, concerning the main objectives.
    * Agreement on a good practice for describing Data Services / APIs.
    * Analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation.
    * Drafting of the Geospatial High-Value Datasets tagging good practice specification.
* Invite participants to actively join the team involved in the lead of the above-mentioned tasks.
* Recap any important decisions taken and trace specific actions for future working team meetings.

The JRC opened the meeting, welcoming the participants and confirming the agenda. 

###  Pilot Phase 2 Working Teams – Objectives & Set up

The JRC delivered a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-26%20-%20T-1B%20Kick-off/presentations/20260226_01_ISO%26GeoDCAT-AP_Pilot_Ph%202-T1-B_Kick_off-JRC.pptx) explaining the purpose of Phase 2 and, more concretely, the different specialised working teams created. These will operate independently but in a coordinated manner:
*	T-1A. Working team focused on managing issues with an impact on geospatial metadata harvesting and reporting of geospatial High-Value Datasets (HVDs), scoped in the integration of INSPIRE geospatial assets into data.europa.eu (hence, highly related to the ISO-to-GeoDCAT-AP mapping and transformation).
*	T-1B (the one kicked-off in this meeting). Working team focused on specific analysis and good practices for the alignment of INSPIRE into data.europa.eu which deserve special attention and/or require substantial effort - mainly highlighting:
    *	Formalisation of the geospatial HVD tagging good practice.
    *	Agreement on a good practice for the description of data service / APIs, and related mapping and transformation issues.
    *	Analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation.
    *	Identification of any remaining gaps and discussion on the need for tackling them.
*	T-2. Working team focused on explore the use of Artificial Intelligence (AI) assisted tools in metadata generation, and other potential uses in metadata management tasks.

The initial plan is to organise working team meetings monthly, supported by continuous coordination, and bi-monthly / quarterly general pilot meetings to exchange progress and updates.

###  T-1B Objectives & Tasks

The JRC gave the floor to the different Member States participants that agreed to lead, with the help and coordination from the JRC, each of the tasks assigned to working team T-1B.

#### Agreement on a good practice for describing Data Services / APIs

FI and DK delivered a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-26%20-%20T-1B%20Kick-off/presentations/20260226_02_ISO%26GeoDCAT-AP_Pilot_Ph%202-T1-B_Kick-GP_Data_Services-APIs-DK_FI_JRC.pptx) to set the scene for agreeing on a good practice for describing Data Services / APIs.

An overview of the task was provided, including the first investigations on the options to establish a mapping for distributions, minimising information loss, and checking that mapping rules and resulting DCAT-files support HVD-reporting. The final objective is to reach an agreement on a good practice on this concern.

The presenters compared and contrasted the different approaches for describing distributions (services / APIs) taken in the [INSPIRE Data-service Linking Simplification Good Practice](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/blob/main/good-practice/data-service-linking-simplification-spec.md) with those in [(Geo)DCAT-AP](https://semiceu.github.io/GeoDCAT-AP/releases/3.1.0/). Afterwards, they made relevant observations related to the transformation from ISO 19139 to (Geo)DCAT-AP, highlighting and discussing several of the issues identified in the context of the pilot.

Subsequently, it was discussed the specific working schedule to discuss with the community and progress on this task, the need to split resposibilities and the convenience to set a repository to share the corresponding materials.

To the fact that the dcat:DataService is only accessible from dcat:Dataset passing through dcat:Distribution, SEMIC (Bert) commented that connecting directly these classes would be a potential future option, if needed. The important thing is that Dataset and DataService are connected via a relationship so that related instances can be queried.

DK (Chirstian) mentioned that, according to his knowledge, the HVD Regulation requires a contact point for the DataService and a permanent reference to it (from the Dataset), which could be complex or pose limitations when connecting dcat:Dataset to dcat:DataService through dcat:Distribution. This could also pose issues when a DataService maintained by one organisation serves Datasets from several other orgnanisations (often the case of INSPIRE catalogues).

BE-Flanders is exploring metadata encoding options in ISO 19139 with the aim to avoid the indetermination of the concrete formats served by specific DataServices / APIs. This country expressed interest in joining this work. NL also expressed interested in joining.

DE expressed difficulties in interpreting the difference between the concept of Distribution and DataService, and would appreciate a common interpretation between data providers / countries.

Finally, the JRC reminded: 
* the importance of participating in the discussion and the provision of feedback on the open issues related to 'Distributions and their mapping in GeoDCAT-AP' - See [Working Team T-1A Kick off Meeting (Action 1)](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-24%20-%20T-1A%20Kick-off%20/readme.md#agreements--actions).
* the need of identifying solutions for countries following either the good practice on Data-service Linking Simplification (from Dataset to DataService) OR the INSPIRE classical Data-service Linking (from DataService to Dataset).

#### Analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation

ES delivered a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-26%20-%20T-1B%20Kick-off/presentations/20260226_03_ISO%26GeoDCAT-AP_Pilot_Ph%202-T1-B_Kick-Mapping_losses_ES_JRC.pptx) on the analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation.

Given the high amount of metadata elements in ISO 19115, the analysis will only consider the most commonly used metadata elements which are absent from GeoDCAT- AP 3.1.0. The work will be organised in two phases: 
* Revision of the ISO 19115 standard (considering mandatory, conditional, and optional metadata elements in this starndard).
* Proposal of suggestions for the ISO-to-GeoDCAT-AP mapping of metadata elements which might be essential, and are missing or are not properly mapped to the target standard.  

The presenters illustrated this work with several examples (EX_VerticalExtent, DQ_DataQuality). 

The JRC (Hagar) expressed interest in contributing to this work, especially in the analysis of the mapping of data quality vocabularies used in both, the ISO 19139 and (Geo)DCAT-AP standards. SEMIC (Bert) clarified that any considerations on this regard should be better captured as guidelines rather than requirements in (Geo)DCAT-AP, to prevent complexity of its scope and facilitate the maintenance of this standard. 

The JRC (Jordi) expressed the convenience of adding, in the transformed GeoDCAT-AP metadata, a pointer to the original ISO 10139 metadata record (at source), to mitigate the impact of potential information losses in the GeoDCAT-AP record. SEMIC (Bert) commented that this would be a useful option, althought it is not clear if the relationship between both, the original and the transformed metadata records, would be always 1:1. This needs to be further analysed.

The JRC highlighted the importance of this task to quantify the loss of information when transforming geospatial / ISO 19139 metadata to (Geo)DCAT-AP, and the fact that this activity may lead to identifying new additional issues in the SEMIC repositories. 

Finally, it was discussed the specific methodology and schedule to progress on this task, inviting other experts ot join the activity.
The work should be finished approximately by the end of June 2026.

#### Drafting of the Geospatial High-Value Datasets tagging good practice specification

IT delivered a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-02-26%20-%20T-1B%20Kick-off/presentations/20260226_04_ISO%26GeoDCAT-AP_Pilot_Ph%202-T1-B_Kick-GP_geospatial_HVD-tagging_spec_IT_JRC.pptx) to describe the pending work for drafting a formal specification for the Geospatial High-Value Datasets tagging good practice agreed during Pilot Phase 1.

The presenters described at high-level the main agreements achieved during Pilot Phase 1, described the objectives for drafing them formally in a good practice specification, and called for contributions in the form of implementation examples and evidences, as well as for volunteers to collaborate in this task. 

The draft specification will be progressing [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/good-practices/hvd-tagging/specification.md).

The work should be finished approximately by the end of June 2026.

The OP (Pavlina) expressed the importance of going further in the geospatial HVD tagging, including both the Category and Subcategory, and an INSPIRE 'label', to support future filtering of geospatial / INSPIRE assets in data.europa.eu, avoding complex queries to find out which assets stems from INSPIRE. 

## Agreements / Actions
- [ ] **Action 1**. All pilot participants to consider joining actively the work of the different team involved in the lead of each T-1B task.
- [x] **Action 2**. All Working Team T-1B sub-groups to start their work right after this Kick-off Meeting.
- [x] **Action 3**. The NL and BE-Flanders to join FI and DK, as part of the team involved in the work for agreeing on a good practice for describing Data Services / APIs.
- [ ] **Action 4**. The JRC to organise a presentation on the work of ISO TC211 on the internal draft of ISO/TS 19115-5, which defines the mapping of ISO metadata to DCAT at global (international) level, in the next General Pilot Meeting.
- [ ] **Action 5**. Member States to share encoding examples and evidences of implementation of the geospatial High-Value Datasets tagging good practice.
