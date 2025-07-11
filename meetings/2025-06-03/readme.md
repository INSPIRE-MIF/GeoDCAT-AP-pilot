# Fifth Pilot Meeting (3 June 2025)

## Agenda

* Overview – Pilot status & progress (JRC) - 15 minutes
    * Ongoing activities.
    * Pilot Final Report (2nd working draft + Final version).
    * 82nd INSPIRE MIG-T Meeting (27 June 2025).
* Pilot issues - 80 minutes
    *	Summary (JRC) - 5 minutes
    * Discussion (selected issues) (All) - 75 minutes
        * Open issues pending from past meeting:
            * [Pilot #3](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/3). Proposal to add hvdCategory as optional to GeoDCAT-AP 3.0 - FI
            * [SEMIC GeoDCAT-AP #143](https://github.com/SEMICeu/GeoDCAT-AP/issues/143). Guidance on the use of prov:qualifiedAttribution on Dataset would be welcome - NL 
        * [Pilot #8](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/8). All formats (gmd:distributionFormat) is listed in each dcat:Distribution - DK
        * [Pilot #9](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/9). Transformation: Distribution, LandingPage and Documentation - FI
        * [Pilot #10](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/10). Proposal to determine distribution format from ISO gmx:mimeFileType - LU
        * [SEMIC GeoDCAT-AP #150](https://github.com/SEMICeu/GeoDCAT-AP/issues/150). Align the usage note about the accessRights property with the proper vocabulary - IT
        * [SEMIC XSLT #64](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/64). Multiple geometry serialisations for dcat:bbox - NL / FI
        * [Pilot #11](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/11). Have you faced issues when transforming service and multilingual metadata? - FI
*	Potential continuation of the pilot - 20 minutes
    * New topic proposal (JRC) - 10 minutes
    * Brainstorming (All) - 10 minutes
* AoB (All) - 5 minutes

## Participants

* Member States: Czech Republic (CZ), Denmark (DK), France (FR), Italy (IT), Finland (FI), the Netherlands (NL), Spain (ES).
* European Commission: Publications Office of the European union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General Joint Research Centre (JRC).
* Contractors: con terra.

## Presentations and recording

Presentations can be downloaded [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/meetings/2025-06-03/presentations).

Recording: Available on request. 

## Meeting summary

The objectives of the meeting were:
* Inform about the status of the ongoing pilot activities, including the Pilot Final report and the geospatial HVD tagging good practice candidate and its potential endorsement by the INSPIRE MIG-T.
* Provide a summary of the pilot issues, its status, and discussion on a selected set of issues (detailed in the agenda).
* Propose possible research topics for a potential continuation of the pilot.
* Agree on the next steps in view of finishing the pilot work by June 2025. 

### Pilot status & progress	

The JRC provided a [short presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2025-06-03/presentations/20250603_01_GeoDCAT-AP_Pilot-00_Overview-JRC.pptx) reporting on the ongoing pilot activities.

* A second draft of the Pilot Final report is available [here](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/final-report).
Additional contributions by participants, particularly to Chapter 6 (Pilot Conclusions), are expected before the next pilot meeting. Deadline traced in the actions.

* The [geospatial HVD tagging good practice candidate](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/good-practices/hvd-tagging) is ready. It will be presented for endorsement at the [82 INSPIRE MIG-T Meeting](https://wikis.ec.europa.eu/spaces/InspireMIG/pages/177046460/82nd+MIG-T+meeting+2025-06-27).

### Pilot issues and relevant discussion	

The participants discussed about the specific issues summarised below:

* [Pilot #3](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/3). Proposal to add hvdCategory as optional to GeoDCAT-AP 3.0 - FI
    * Discussion was continued to assess the appropriateness of transforming HVD Categories values in a conditional manner, depending on the existence of a value citing the HVD ELI code (similarly to how it is already being done by Con Terra’s XSLT), potentially as an extended profile.
    * A basic transformation could only consider transforming the HVD category value when the HVD ELI code is present but there was a call to incorporate these to GeoDCAT-AP, considering that the many of the list’s concepts are geospatial. IT noted that the need to provide documentation for providing and transforming the categories is also need for instance of services as in [Add 'HVD category' and 'documentation' properties related to high-value datasets · Issue #147 · SEMICeu/GeoDCAT-AP](https://github.com/SEMICeu/GeoDCAT-AP/issues/147).

* [SEMIC GeoDCAT-AP #143](https://github.com/SEMICeu/GeoDCAT-AP/issues/143). Guidance on the use of prov:qualifiedAttribution on Dataset would be welcome - NL
    * Agreement was reached to improve the documentation stating that GeoDCAT-AP direct properties take precedence over the use of the prov:qualifiedAttribution construct.
    * SEMIC will include this in the next GeoDCAT-AP draft.
      
* [Pilot #8](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/8). All formats (gmd:distributionFormat) is listed in each dcat:Distribution - DK
    * The issue addressed the challenge when wishing to map formats encoded via ISO/INSPIRE to DCAT because in ISO, the formats are not directly linked to a given resource. The issue was also raised by FI in the relevant ISO repository but no clear suggestions are currently available.
    * The issue would be better solved by ISO TC211 in a future revision of ISO 19115.
    * con terra noted that a similar mismatch of granularity level can create issues when transforming licences.
    * See related issue below.

* A related issue - [Pilot #10](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/10). Proposal to determine distribution format from ISO gmx:mimeFileType – LU
    * It could be used to resolve the issue on a technical level. However, on a semantic level the use of gmd:name (and associated gmx:mimeType) does not appear to convey the same meaning.
    * NL mentioned another related issue: [mapping of Distribution and DataService #59](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/59) (SEMICeu/iso-19139-to-dcat-ap).
    * DK noted that because of the technical requirements of INSPIRE there may be a need to preserve the information on the dataset level, potentially repeating the information mapped to dcat:Distributions.
    * It was generally agreed that resolution of these issues will also require revisiting the INSPIRE guidelines.
  
* [Pilot #9](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/9). Transformation: Distribution, LandingPage and Documentation - FI
    * Currently, only resources that have capabilities and/or are defined as “download” are mapped to distributions (and potentially linked services).
    * The issue is related to the previous ones and a call was made to continue analysing the issue and identify possible strategies to address it.

* [SEMIC GeoDCAT-AP #150](https://github.com/SEMICeu/GeoDCAT-AP/issues/150). Align the usage note about the accessRights property with the proper vocabulary - IT
    * The issue notes inconsistencies between (1) documentation on use of the INSPIRE and OP vocabularies in the GeoDCAT-AP documentation and (2) between DCAT-AP and GeoDCAT-AP.
    * Pending additional feedback, an agreement was reached that the INSPIRE code list can be mapped the OP list, essentially reducing the cases covered by the INSPIRE code list to “public”, “restricted” and “non-public”.

* [SEMIC XSLT #64](https://github.com/SEMICeu/iso-19139-to-dcat-ap/issues/64). Multiple geometry serialisations for dcat:bbox - NL / FI
    * With regards to the current transformation of ISO spatial extent as both locn:geometry and dcat:bbox attributes of locations, this should be revisited and only the latter one kept.
    * The second point, whereby the geometries are serialised in various datatypes, participants did not have a specific preference which serialisation should be preferred if only a single type is to be maintained.
    * con terra informed the group that the choice of a single datatype, as done by the geoharveter of the European data portal, was a technical choice and only exposes the coordinates available in the ISO metadata. 

* [Pilot #11](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/issues/11). Have you faced issues when transforming service and multilingual metadata? - FI
    * Called for feedback of issues detected when transforming multilingual datasets, depending on the use of the core or extended profile. 

### Potential continuation of the pilot

* The JRC delivered a presentation to propose possible research topics for a potential continuation of the pilot. Particularly, a proposal for developing an Artificial Intelligence (AI)-powered metadata editor for geospatial data, which could help simplifying certain metadata management activities.
  
* Participants provided feedback, and gave additional ideas to support specific technical tasks: data-service linking simplification, geo-HVD tagging good practice, metadata encoding changes,                finetuning of codelists, language-related transformations.

## Actions

The following agreements were reached between the pilot participants.
* DK, ES, IT, FI and NL volunteered to help drafting the Chapter 6 (Pilot Conclusions) ofthe Pilot Final report-
* Volunteers to revise the [second draft of the final report](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/tree/main/final-report) and provide contributions by 19 June 2025.
* Update the status of the issues discussed in this meeting.
* The next (Sixth) meeting of the pilot ideally will take place in the week from 16 to 20 June 2025, depending on participants' availability.
