# Second Pilot Meeting (20 November 2024)

## Agenda

*	Introduction (JRC)
    * Meeting objectives & Timeline recap
*	Pilot progress (participants: BE-Flanders, DK, IT, FI, NL, ES, SK-presented by JRC, OP, JRC)
    *	Testing focus (Specification and/or Transformation)
    * Progress achieved / Issues
    * Expectations / Proposals
*	Specific pilot bits.
    * ISO metadata High-Value Datasets tagging practices (JRC)
    * Approaches to run the XSLT transformation (TBD)
    * Discussion
* Pilot progress report (80th MIG-T Meeting) (All)
* Management of pilot materials. Next meeting & Wrap up (JRC)
* AoB (All)

## Participants

* Member States: Belgium (BE-Flanders), Denmark (DK), Italy (IT), Finland (FI), the Netherlands (NL), Spain (ES).
* European Commission: Publications Office of the European union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General for Environment (ENV), Directorate-General Joint Research Centre (JRC).
* Contractors: conterra.

NOTE: CZ and SK excused their attendance to this metting due to its overlap with the Czech–Slovak INSPIRE Conference.

## Presentations and recording

Presentations can be downloaded [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2024-11-20/presentations).

Recording: Available on request. 

## Meeting summary

The objective of the meeting was to have the first working exchange between pilot participants, with the following plan:
* Clarify any aspects from the [Kick-off Meeting](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2024-10-02) (2024-10-02).
* Evaluate the progress achieved by each participant.
* Exchange information and discuss on specific bits concerning the pilot.
* Decide how to report about the pilot in the [80th INSPIRE MIG-T Meeting](https://wikis.ec.europa.eu/display/InspireMIG/80th+MIG-T+meeting+2024-12-13) (2024-12-13).
* Share news on the [INSPIRE GeoDCAT-AP Pilot management repository](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/).

### Pilot progress reports
Each participant presented a short report on the their progress, including a description of their main testing focus (specification and/or XSLT transformation), the progress achieved and the issues identified until the date. They also raised specific highlights, expectations on the pilot and related proposals (if any).
Check the [pilot progress presentations](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2024-11-20/presentations) for more details.

### Relevant discussion	

The participants discussed about the specific pilot bits summarised below:

* ISO metadata High-Value Datasets (HVDs) tagging practices
  * Several encoding examples for tagging High-Value Datasets (from BE-Flanders, DE, DK, ES and NL) were shared across participants. They use different types of encodings (CharacterString vs. Anchor approaches). The input examples are available [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/good-practices/hvd-tagging/inputs).
  * The SEMIC XSLT transformation needs to be updated based on an harmonised way for tagging HVDs. This will be the basis for applying the specific (additional) requirements stemming from the [HVD Implementing Regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32023R0138), further specified within the [DCAT-AP High Value Datasets usage guidelines](https://semiceu.github.io/DCAT-AP/releases/3.0.0-hvd/).

* Parallel ‘DCAT-AP schema plugin integration in GeoNetwork’ Working Group
  * A joint effort to integrate a DCAT-AP / GeoDCAT-AP schema plugin in GeoNetwork is ongoing.
  * This working group, organised by BE-Flanders and the GeoNetwork community, has already implemented a DCAT-AP (v2) plugin for the GeoNetwork Core, and the plan is to extend it to GeoDCAT-AP and the v3 of the standards.
  * The ad-hoc repository for this work is available [here](https://github.com/orgs/metadata101/projects/2).
  * Next sprints are scheduled on 25-27 November 2024 (Sprint 3), and 9-11 December (Sprint 4).
  * The ISO & GeoDCAT-AP pilot participants are invited to join.

* [data.europa.eu](https://data.europa.eu/en) (DEU) Geo-harvester
  * The Geo-harvester currently maps ISO 19139 geospatial metadata to [GeoDCAT-AP 2](https://semiceu.github.io/GeoDCAT-AP/releases/2.0.0/).
  * The plan is to update this mapping to [GeoDCAT-AP 3](https://semiceu.github.io/GeoDCAT-AP/releases/3.0.0/) approximately by January 2025. conterra (contractor operating DEU) offers the possibility to any interested stakeholder for testing this new mapping when available.
  * The OP is currently discussing with conterra the specific mappings for appropriately identifyng HVDs and the HVD Categories. These mappings will determine the basis for HVDs filtering in DEU.

* Potential integration of pilot issues / outcomes
  *  FI proposed to use [this GitHub repository](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues) for sharing the initial issues and outcomes from pilot participants, with the aim of analysing their potential integration before sharing them with SEMIC.

* Approaches to run the XSLT transformation
  * Participants reported on the use of different tools to run the XSLT transformation: GeoNetwork, Saxon, SEMIC Proof-of-Concept (PoC) API, XMLSpy, custom tools (command line / Python), DEU Geo-harvester. Check the [progress presentations](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2024-11-20/presentations) for more details.


## Actions

The following agreements were reached between the pilot participants.
* In the context of the next sprints of the 'DCAT-AP schema plugin integration in GeoNetwork’ Working Group, analyse the different HVDs tagging practices identified until the date with the aim to discuss and propose a candidate implementation good practice. The objective is to present the proposal in the [80th INSPIRE MIG-T Meeting](https://wikis.ec.europa.eu/display/InspireMIG/80th+MIG-T+meeting+2024-12-13), possibly for initiating its potential endorsement.
* Participants to consider the use of [this GitHub repository](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues) for sharing the initial issues and outcomes stemming from the pilot, for their potential discussion and integration with the rest of participants.
* Analyse the [pilot progress presentations](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2024-11-20/presentations) summarising the results achieved by participants until this meeting (Summary available [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2024-11-20/GeoDCAT-AP_Pilot-Second_Meeting-Progress_summary.pdf)).
* BE-Flanders volunteered to help JRC in reporting about the pilot progress in the [80th INSPIRE MIG-T Meeting](https://wikis.ec.europa.eu/display/InspireMIG/80th+MIG-T+meeting+2024-12-13).
* Third Meeting of the pilot to be scheduled by sending a poll with option dates starting from 12 December 2024.
