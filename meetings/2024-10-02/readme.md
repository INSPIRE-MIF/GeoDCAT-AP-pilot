# Pilot Kick-off Meeting (2 October 2024)

## Agenda

* Introduction
* Pilot proposal
    * Objectives (General & Specific)
    * Structure & Participants
    * Outputs
    * Timeline (General & Specific)
* Refinements (discussion)
* Final proposal & Pilot work start (target date)
* Next meeting
* AoB.

## Participants

* Member States: Belgium (BE-Flanders), Czech Republic (CZ), Denmark (DK), Italy (IT), Finland (FI), the Netherlands (NL), Spain (ES), Slovakia (SK).
* European Commission: Publications Office of the European union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General Joint research Centre (JRC).

## Presentations and recording

[Kick-off meeting Presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2024-10-02/presentations/20241002_GeoDCAT-AP_Pilot_KoM_v6.pdf) (JRC)

NOTE: recording not available due to technical difficulties with Webex. 

## Meeting summary

The objective of the meeting was to lauch the ISO & GeoDCAT-AP pilot, present a first work proposal and refine it in agreement with the participants. 

### Introduction & Pilot proposal

A presentation was delivered by the JRC including an introduction contextualising the pilot, the participants who volunteered to take part of the exercise (BE (Flanders), CZ, DK, IT, FI, NL, ES, SK, as well as OP, SEMIC and JRC), the general and specific objectives of the pilot, an enumeration of the expected outcomes and an initial timeline (from October 2024 until mid-November).

Check the presentation for further details.

### Relevant discussion

* A representative from DIGIT-SEMIC suggested using the [GeoDCAT-AP repository](https://github.com/SEMICeu/GeoDCAT-AP/issues) to gather the pilot issues on the specification, while using the [XSLT repository](https://github.com/SEMICeu/GeoDCAT-AP/issues) to gather the pilot issues on the transformation.
* This representative also clarified that the tags to classify the issues stemming from the pilot in the SEMIC repositories would be managed by the repository maintainers (SEMIC), and proposed a common shorter tag for this purpose.  
* Conterra GmbH, on behalf of the OP, raised that currently the CSW interface of the data.europa.eu Geoharvester is only supporting [GeoDCAT-AP 2](https://semiceu.github.io/GeoDCAT-AP/releases/2.0.0/), and that the resources to update it to support [GeoDCAT-AP 3](https://semiceu.github.io/GeoDCAT-AP/releases/3.0.0/) still need to be allocated.
* A representative from FI mentioned that some issues regarded to the pilot were already open in the [GeoDCAT-AP](https://github.com/SEMICeu/GeoDCAT-AP/issues) repository before this Kick-off Meeting. They will have to be identified and appropiately tagged based on the outcomes of the meeting.
* A representative from DK asked if the GeoDCAT-AP 3 spec was also mapped to the new [ISO 19115-3](https://www.iso.org/standard/80874.html) standard – The answer was NOT, but it was highlighted the fact that an annex is provided in the GeoDCAT-AP 3 specification explaining the main differences of this new version of the standard with respect to the [ISO 19115:2003](https://www.iso.org/standard/26020.html) standard (the version that the GeoDCAT-AP 3 specification maps to).
* Representatives from BE-Flanders and IT raised concerns with the proposed timeline – A more relaxed timeline will be agreed in the coming days, probably ending by February 2025, rather than by December 2024. This will also avoid interferences with the on-going and parallel work to develop a GeoNetwork schema plugin for [GeoDCAT-AP 2](https://semiceu.github.io/GeoDCAT-AP/releases/2.0.0/). That working group will tackle the plugin for [GeoDCAT-AP 3](https://semiceu.github.io/GeoDCAT-AP/releases/3.0.0/) in the future. 
* A representative from ES asked if there were examples on additional tagging of HVDs, apart from the INSPIRE themes mapping to HVDs categories – Answer was YES. Examples will be shared together with the Kick-off presentation.  

## Actions

It was agreed to consider all the points raised, integrating them in the proposal and updating the Kick-off Meeting presentation for further reference ([latest version: v6](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2024-10-02/presentations/20241002_GeoDCAT-AP_Pilot_KoM_v6.pdf)).

Particularly: 
* Repositories to report the issues stemming from the pilot (they will be tagged by SEMIC using the ‘3.0.0 Pilot’ tag):
    * Issues on the GeoDCAT-AP 3 specification: to be reported at https://github.com/SEMICeu/GeoDCAT-AP/issues
    * Issues on the related XSLT transformation: to be reported at https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues
* Any already reported issues will be tagged by SEMIC using the mentioned tag in the previous repositories.
* An updated, more relaxed, timeline has been agreed:
    * Starting from 2nd October 2024 (Kick-off meeting)
    * Working Group Testing: October 2024 - January 2025.
    * Collection of feedback and results: until End of January 2025.
    * Final report compilation: until End of February 2025.
    * Potential GeoDCAT-AP 3 updates: to be considered from March 2023.
* Examples of good practices for tagging High-Value Datasets (HVDs) in geospatial ISO metadata will be shared with the pilot participants and the rest of the INSPIRE community.
