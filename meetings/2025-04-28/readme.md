# Fourth Pilot Meeting (28 April 2025)

## Agenda

* Overview – Pilot status & progress (JRC) - 15 minutes
    * Ongoing activities.
    * Pilot Final Report (1st working draft).
    * High-Value Datasets (geospatial) tagging good practice candidate.
        * Voting results & potential INSPIRE MIG/MIG-T endorsement.
* Harvesting in [data.europa.eu](https://data.europa.eu/en) – How does it work? (OP / con terra) - 15 minutes
* Pilot issues - 65 minutes
    *	Summary (JRC) - 5 minutes
    * Discussion (selected issues) (All) - 60 minutes
        * [Pilot #2](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/2). Proposals related to the HVD tagging good practise and the XSL transformation - FI
        * [Pilot #4](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/4). Role of service metadata in the EDP, in HVD-reporting and in this pilot? - FI
        * [Pilot #3](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/3). Proposal to add hvdCategory as optional to GeoDCAT-AP 3.0 - FI
        * [SEMIC GeoDCAT-AP #143](https://github.com/SEMICeu/GeoDCAT-AP/issues/143). Guidance on the use of prov:qualifiedAttribution on Dataset would be welcome - NL
        * GeoDCAT-AP mapping / Extended mapping:
            * [SEMIC XSLT #70](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/70). gmd:purpose -> how to map? (suggested also to dct:description) - DK
            * Mapping: GMD optional attributes not mapped to geoDCAT - ES
        * Useful to have a common place to share national XSLTs for local uses - FR  
*	Pilot way forward (All) - 15 minutes
    * Brainstorming
* DCAT-AP schema plugin for GeoNetwork – Updates (BE Flanders) - 5 minutes
* AoB (All) - 5 minutes

## Participants

* Member States: Belgium (BE-Flanders), Czech Republic (CZ), Denmark (DK), France (FR), Finland (FI), the Netherlands (NL), Spain (ES).
* European Commission: Publications Office of the European union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General Joint Research Centre (JRC).
* Contractors: con terra.

## Presentations and recording

Presentations can be downloaded [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2025-04-28/presentations).

Recording: Available on request. 

## Meeting summary

The objectives of the meeting were:
* Inform about the status of the ongoing pilot activities, including the Pilot Final report and the geospatial HVD tagging good practice candidate.
* Explain how the harvesting in [data.europa.eu](https://data.europa.eu/en) with a detailed presentation delivered by con terra/OP.
* Provide a summary of the pilot issues, its status, and on a selected set of issues (detailed in the agenda).
* Provide and update of the work of the DCAT-AP schema plugin for GeoNetwork working gorup lead by BE-Flanders.
* Agree on the next steps in view of finishing the pilot work by June 2025. 

### Pilot status & progress	

The JRC provided a short presentation reporting the ongoing pilot activities.

* A first draft of the Pilot Final report is available [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/final-report).
Additional contributions by participants, particularly to each participant's seccion in Chapter 3 and 4, are expected before the next pilot meeting. Deadline traced in the actions.

* The [geospatial HVD tagging good practice candidate](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/good-practices/hvd-tagging) is ready. After the conciliation meetings with Member States which expressed concerns about the good practice, the whole 19 Member States which participated in the consultation voted positively. The plan is to present this good practice candidate for endorsement in the [82 INSPIRE MIG-T Meeting](https://wikis.ec.europa.eu/spaces/InspireMIG/pages/177046460/82nd+MIG-T+meeting+2025-06-27).

### Harvesting in [data.europa.eu](https://data.europa.eu/en)	

con terra delivered on behalf of the OP a presentation explaining how the harvesting in [data.europa.eu](https://data.europa.eu/en) works, including a detailed description of the harvesting process, where the transformation to GeoDCAT-AP takes place, the role of the Geoharvester in the workflow, and the capabilities of this component.

Some Geocatalogues harvest other (lower-level) geocatalogues and are afterwards harvested by the national Open Data catalogue. This led to some confusions in the past. 
In short, if a Geocatalogue is harvested directly by data.europa.eu, there is no need to apply the transformation by the MS. This is done by data.europa.eu directly.

This situation does not help in preventing “metadata duplicates” in data.europa.eu - e.g. in DE both gov.data (Open Data catalogue) and the Geocatalogue are harvested. gov.data partially harvests the geocatalogues. Therefore, this could create some duplications. In such cases, it is not easy to decide which source is preferable. Preventing this problem in the future is a subject of study.

The Geoharvester has been already updated to comply to GeoDCAT-AP 3 and is now able to process the geospatial HVD taging good practice candidate, and is available in the development environment. conterra tested with this system the catalogues from participating MSs in this environment, noting whether HVDs were detected or not. Any feedback from participating MSs is welcome.

con terra reported two old-known issues concerning to metadata quality / encoding issues in data.europa.eu (detailed in the presentation). These are not traced on GitHub, but explained in the presention for helping MSs to avoid them in their metadata records.

The presentation is available [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2025-04-28/presentations/20250428_02_Harvesting_in_data.europa.eu-OPconterra.pdf).

NL asked if the SEMIC and the data.europa.eu XSLT transformations are the same - conterra clarified that there are some differences, mainly pertaining to the inclusion of Service metadata. 

### Pilot issues and relevant discussion	

The JRC presented an [Excel spreadsheet](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/final-report/ISO-GeoDCAT-AP_Pilot_issues_v1_20250428.xlsx) summarising the Pilot issues received so far, showing its status.

Many issues have been already identified to be ready for their submission to SEMIC. On the other hand, a selected set of issue were selected for discussion in this meeting (detailed in the agenda and in the discussion overview below).

The participants discussed about the specific topics summarised below:

* [Pilot #2](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/2). Proposals related to the HVD tagging good practise and the XSL transformation - FI
    * Answers to the two proposals raised in this issue thread were given.
    * A pending topic - to be clarified and discussed within the INSPIRE community - is how refer in the future to other legislations, such as the ones from the PriorityDatasets codelist, in GeoDCAT-AP. This is the main purpose of [this separated thread](https://github.com/INSPIRE-MIF/helpdesk-registry/issues/115).
  
* [Pilot #4](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/4). Role of service metadata in the EDP, in HVD-reporting and in this pilot? - FI
    * The different views expressed in this issue thread were further explained and clarified.
    * A remark for further reflection - In the [DCAT-AP High Value Datasets](https://semiceu.github.io/uri.semic.eu-generated/DCAT-AP/releases/2.2.0-hvd/) metadata profile there is a clear encouragement to mark the service metadata. The INSPIRE community should discuss how to do this.
    * SEMIC stressed the importance of APIs in the HVD Implementing Regulation, and that this is translated into the concept of 'data service'. Thus, these services should be subject to search and be appropiately described with metadata within HVD reporting. If the API / data service is considered as a distribution, it will no be appearing in the HVD reporting and therefore not shown as an API. 
    * Further guidance and discussion is needed on how to represent HVD services in INSPIRE metadata. The importance of encoding them as sevices is ackownledged.
    * A [Beta version tool](https://data.europa.eu/apps/hvd-reporting-tool/detail.html) is available in data.europa.eu to help MS to report an comply with HVD reporting obligations. The tool is not fully complete yet and will be improved in the future. The objective is that, for every national catalogue, it will be possible to check the status of the HVD reporting obligations for corresponding country.
  
* [Pilot #3](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/3). Proposal to add hvdCategory as optional to GeoDCAT-AP 3.0 - FI
TBC
  
* [SEMIC GeoDCAT-AP #143](https://github.com/SEMICeu/GeoDCAT-AP/issues/143). Guidance on the use of prov:qualifiedAttribution on Dataset would be welcome - NL
TBC

* GeoDCAT-AP mapping / Extended mapping:
    * [SEMIC XSLT #70](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/70). gmd:purpose -> how to map? (suggested also to dct:description) - DK
      TBC

    * Mapping: GMD optional attributes not mapped to geoDCAT - ES
      TBC

* Useful to have a common place to share national XSLTs for local uses - FR
TBC  

###  DCAT-AP schema plugin for GeoNetwork – Update 

BE-Flanders provided an update of the activities of the 'DCAT-AP schema plugin integration in GeoNetwork’ Working Group. 
The presentation is available [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2025-04-28/presentations/20250428_03_DCAT_Schema_Plugin_WG_update-BE_Flanders.pptx).

## Actions

The following agreements were reached between the pilot participants.
* Each participant to revise the [first draft of the final report](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/final-report) and provide contributions by 21 May 2025.
* The next (Fifth) meeting of the pilot ideally will take place in the week from 26 to 30 May 2025, depending on participants' availability.
* TBC
