 # Pilot Phase 2 - Working Team T-2 Kick-off meeting (13 March 2026)

## Agenda
*	Welcome
*	Pilot Phase 2 Working Teams - Objectives & Set up (JRC) - 10 minutes
*	T-2 Objectives, Strategy & Tasks (JRC / OP / SEMIC) - 10 minutes 
    *	Discussion (All) ~ 20 minutes
*	AI- assisted metadata generation tool (JRC) - 20 minutes
    *	Discussion (All) ~ 20 minutes
*	Summary of actions from the meeting (JRC) - 10 minutes
*	AoB (All)

## Participants

* Member States: Belgium (BE-Flanders), Croatia (HR), Czech Republic (CZ), Denmark (DK), Latvia (LV), Finland (FI), France (FR), Germany (DE), Malta (MT), the Netherlands (NL), Spain (ES).
* European Commission: Publications Office of the European Union (OP), Directorate-General for Digital Services SEMIC Group (DIGIT-SEMIC), Directorate-General Joint Research Centre (JRC), the European Environment Agency (EEA).
* Contractors: con terra, Epsilon Italia.

## Presentations and recording

Presentations can be downloaded [here]().

Recording: Available on request. 

## Meeting summary

The objectives of the meeting were:
* Explaining the purpose of Phase 2 and why specialised working groups are needed.
    * Generally define the scope, expected deliverables and timelines for each working team (T-1A, T-1B, T-2).
    * Clarify the working plan (independent work with regular cross‑team coordination) and potential interactions between them.
* Describe the tasks assigned to working team T-2, concerning the main objectives.
    * Exploration and testing of AI-assisted tools for metadata generation, in particular the exisiting prototype by the JRC.
    * Identification of other areas where AI-assisted tools may be used to support metadata management.
    * Other objectives yet to be identified and discussed, depending on the outcomes of the above-mentioned results.
* Invite participants to actively join the team involved in the lead of the above-mentioned tasks.
* Recap any important decisions taken and trace specific actions for future working team meetings.

The JRC opened the meeting, welcoming the participants and confirming the agenda. 

### Pilot Phase 2 Working Teams – Objectives & Set up

The JRC delivered a [presentation](https://github.com/INSPIRE-MIF/GeoDCAT-AP-pilot/blob/main/meetings/2026-03-13%20-%20T-2%20Kick-off/presentations/20260313_01_ISO%26GeoDCAT-AP_Pilot_Ph%202-T2_Kick_off-JRC.pptx) explaining the purpose of Phase 2 and, more concretely, the different specialised working teams created. These will operate independently but in a coordinated manner:
*	T-1A. Working team focused on managing issues with an impact on geospatial metadata harvesting and reporting of geospatial High-Value Datasets (HVDs), scoped in the integration of INSPIRE geospatial assets into data.europa.eu (hence, highly related to the ISO-to-GeoDCAT-AP mapping and transformation).
*	T-1B. Working team focused on specific analysis and good practices for the alignment of INSPIRE into data.europa.eu which deserve special attention and/or require substantial effort - mainly highlighting:
    *	Formalisation of the geospatial HVD tagging good practice.
    *	Agreement on a good practice for the description of data service / APIs, and related mapping and transformation issues.
    *	Analysis of potential metadata information losses in the ISO-to-GeoDCAT-AP transformation.
    *	Identification of any remaining gaps and discussion on the need for tackling them.
*	T-2 (the one kicked-off in this meeting). Working team focused on explore the use of Artificial Intelligence (AI) assisted tools in metadata generation, and other potential uses in metadata management tasks.

The initial plan is to organise working team meetings monthly, supported by continuous coordination, and bi-monthly / quarterly general pilot meetings to exchange progress and updates.

#### T-2 Working Team – Objectives

Subsequently, a discussion was held on additional objectives for T-2:

* SEMIC is very active in AI for semantics, as well as semantics for AI. In that area, SEMIC is currently running pilots for semantic tagging using Large Language Models (LLMs), and also developing ChatBots (as a proof of concept) to support semantic modelling. Although being more active in T-1A & T-1B Working Teams, SEMIC will try to support the activity of this working team as much as possible, depending on the needs identified. 

* OP is willing to support data providers in the annotation process and validate metadata using AI and other useful tools, with the aim to avoid errors and increase quality of the metadata records harvested in data.europa.eu.

* JRC commented that Member States may find useful such kind of tools, especially if they simplify their daily management tasks.
  
* Both, SEMIC and OP, are willing to explore the opportunities for simplifying metadata management with AI, but will be willing to concrete those once the needs from Member States are more clearly identified in a later stage of the pilot working team.

* The EEA is interested in going in production with tools that help them populate metadata, relatively quickly, by the end of 2027. They are exploring with Model Context Procolol (MCP) that enables the AI to generate and maintain metadata working from their GeoNetwork catalogue, and offered the possibility to share the corresponding code. The main concern of EEA is how to make sure the AI-generated metadata have enough quality (content, keywords, etc.), especially when generating new records, and are looking for existing solutions to control it.  

### AI-assisted metadata generation tool (JRC)

The JRC (Margherita) delivered a nice demonstration of the metadata generation tool prototype that has been developed internally. The intention is to test it with real users (e.g., Member States) that are willing to explore it with the aim of enhancing the prototype.

The prototype supports the creation of geospatial metadata in GeoDCAT-AP, semi-automating these tasks based on a set of supporting materials and refining the output metadata with a human expert in the loop. The app relies on an Agentic AI architecture using the Model Context Protocol (MCP), and Python tools activated by the AI when needed. A web user interface is used to upload input materials (dataset, supporting documents, etc.) and interact with the system for refining the metadata.
The intention is to offer this tool as open source when enough tested.

The demo was video recorded and is available on demand.

The EEA was interested on how to prevent AI hallucinations and explicitly asked about the methodology used to investigate the best prompting strategies. The JRC clarified that several prompting techniques were aanlysed and compared (object of an article recently submitted). Quality of results strongly depends on the LLMs. There is a need to test the tool with real examples to analyse and enhance the quality of the metadata being produced.

JRC clarified that the input data provided to the LLM needs to be correct, and this is responsibility of the human / expert which stays in the loop. 

The EEA also commented the need to generate user-friendly descriptions in the metadata, avoiding acronyms, technicisms, etc. The JRC commented that soem of these aspects can be controlled via prompting (e.g., explanation of acronyms, use of simpler synonyms, etc.).

BE-Flanders asked if the prototype is transparent in reporting how the metadata was generated, e.g. if AI was been used, and in which percentage it was used to generate metadata elements. The JRC commented this would be technically possible but it should be discussed how to report this information in the metadata standards. At the moment, it is not regulated. It was also mentioned the convenience to raise this question to standardisation bodies (ISO / OGC). The next OGC Europe Forum in Helsinki (June 2026) will be a nice opportunty to discuss this topic.

JRC commented that AI-assisted tools might be useful to support the tagging of geospatial metadata, enhance it, with special focus on HVD reporting. BE-Flanders supported this idea.

Finally, the JRC invited the pilot participants to test the prototype tool and provide expert feedback on this solution. This might help defining new research directions and create opportunities for supporting future metadata management activities.  

## Agreements / Actions

- [ ] **Action 1**. All pilot participants to consider joining actively the work of the working team T-2.
- [ ] **Action 2**. BE-Flanders, DE, and the EEA expressed interested in testing the metadata generation tool prototype. They will be contacted as soon as the testing architecture is ready to start the activity. The invitation for testing will be kept open to other participants.
