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

TBC
* Member States: .
* European Commission: .
* Contractors: .

## Presentations and recording

TBC 

## Meeting summary

TBC



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

## Actions

The following agreements were reached between the pilot participants.
* TBC
