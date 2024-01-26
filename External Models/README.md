
# External Conceptual Models and Ontologies

Please add to this list any external models that are being used in this work:

```The format for this list is still to be defined - we need names and links - but it would also be useful to have comments and links to which local models these external models are used in.```

### PIDINST
Research Data Alliance (RDA)
Persistent Identification of Instruments (PIDINST)
working group output report
https://docs.pidinst.org/en/latest/white-paper/metadata-schema.html


## CIDOC CRM

[CIDOC CRM](https://www.cidoc-crm.org/) is a high-level ontology for the humanities that is increasingly used for heritage science data. The “CRM” stands for “conceptual reference system”. It sees the world as a series of events, i.e. meetings of people, ideas and objects, which interact with each other in limited areas of space, time and periods, and bring about noteworthy changes. 
A short introduction to CIDOC CRM is in the [CIDOC CRM folder](CIDOC_CRM). 

CIDOC CRM is also called CRMbase to distinguish it from its domain-specific extensions.

### SSHOCro

SSHOCro, which stands for “SSHOC Reference Ontology”, is a CIDOC CRM extension that was developed within SSHOC by FORTH. It models the lifecycle of SSH data and extends the reach of CIDOC CRM into the social sciences. SSHOCro has a few basic concepts:
* SSH Project (with a project status and a work plan)
* Knowledge Workflow Activity (KWA), which models a common order of work steps in scientific
research:
  1. data collection,
  2. data preparation/processing and connecting different datasets,
  3. interpretation, including writing reports.
* auxiliary activities: 
  1. data storage,
  2. publication of data, reports etc.
* Dataset: the main inputs and outputs of the Knowledge Workflow Activity steps
* Service and Tool.

More details can be found in the [SSHOCro folder](CIDOC_CRM/SSHOCro).


## HESCIDA (KIK/IRPA)

HESCIDA is an E-RIHS.be project lead by KIK-IRPA that aims to create a heritage science knowledge base with art historical, conservation/restoration and material data. 
It builds on the existing BALaT portal hat contains a unique collection of over 850 000 photos of Belgian heritage, an authority list of persons & institutions, and the library catalogue. 
A vast treasure of archives remained however undisclosed. Almost 20 000 intervention files since the inception of KIK/IRPA contain evidence of a rich past and present in the research and 
treatment of numerous heritage objects: condition, conservation, restoration and laboratory reports, detailed images taken during restoration, samples, analytical data... HESCIDA will
provide tools to document this data and to disclose it in BALaT and a repository.

The HESCIDA stack will consist of several tools. The art-historical data, persons & institutions database and library collection are managed by a commercial collection management system,
currently Adlib and in the near future Axiell Collections. Images are served by a IIIF-server and will by managed by a bespoke digital assets management system (DAMS). All other datasets 
are being collected in a centralised file archive, and will be documented with Metahub. This bespoke metadata collector platform will allow researchers to manage and document intervention 
files, reports, analytical datasets, samples and sample collections. In doing so, links will be made between those entities and with the entities stored in the other data sources.

Due to the widely differing metadata that needs to be stored in Metahub and the need to create a user-friendly environment for the researchers, a versatile mechanism is implemented in 
Metahub: 4 basic models are created: projects (including intervention files), datasets (reports, scientific imaging, analytical data), samples and sample collections. These 4 models 
only contain the most rudimentary metadata that is required for the proper functioning of the software. Each of those basic models can be extended to cater for specific needs in two tiers.
The first tier, categories, are meant to define universal metadata schemas, while the second tier, templates, are used to define very specific schemas.

An example of a category is a metadata schema for Raman spectroscopy. Many heritage science institutions have one or more systems, in different set-ups. Using the [category schema for Raman spectroscopy](HESCIDA/raman.schema.json), it should be able to document any Raman spectrum, whereever it was created, whatever instrument was used. 
This scheme does not arise out of nowhere, but is heavily influenced by the [metadata schema](http://irug.org/uploads/documentation/irug-jcamp-dx-revised-white-paper-text-only-with-2b-version-1-26-sept-2013.pdf) 
developed by the [IRUG](http://irug.org/) community. The IRUG metadata is part of the specification to store data and metadata in the open JCAMP-DX format. The focus of IRUG, however, is
on reference samples, and is not well adapted for more complex sample types. Sample metadata is not included in the HESCIDA Raman metadata schema, but documented in a separate, linked
entity.

An example of a template is a [metadata schema for a Raman spectroscopy experiment, conducted with the Renishaw InVia, equiped with a NIR 785nm laser](HESCIDA/raman_invia785.schema.json). The template metadata schema contains a specific set-up at KIK/IRPA, with many fields having precise predefined values. This eases the researcher in 
documenting the experiments.

Currently, the following metadata schemas are uploaded into the HESCIDA subfolder
- [raman.schema.json](HESCIDA/raman.schema.json): generic metadata schema for Raman spectroscopy experiments
	- [raman_invia785.schema.json](HESCIDA/raman_invia785.schema.json): specific schema for an often used set-up at KIK/IRPA
- [dendro.schema.json](HESCIDA/dendro.schema.json): generic metadata schema for dendrochronology analysis
	- [dendro_kikirpa.schema.json](HESCIDA/dendro_kikirpa.schema.json): specific schema for dendrochronology at KIK/IRPA
- [drms.schema.json](HESCIDA/drms.schema.json): generic metadata schema for drilling resistance measurements
(more will be added)

Note: these are draft schemas, and we welcome comments and contributions


## PARTHENOS PROJECT

PARTHENOS project – “Pooling Activities, Resources and Tools for Heritage E-research Networking, Optimization and Synergies” was funded by European Commission under the
[H2020 – EU.1.4.1.1. – Developing new world-class research infrastructures](https://cordis.europa.eu/programme/id/H2020_INFRADEV-4-2014-2015) call with the scope of supporting 
the construction and operation of the research infrastructures identified in the ESFRI Roadmap, as well as other world class research infrastructures, in a specific thematic
area of high priority. The consortium involved 15 partners, as national research organisations, cultural heritage institutions and existing Research Infrastructures,
(http://www.parthenos-project.eu).
PARTHENOS aimed at strengthening the cohesion of research in the broad sector of Linguistic Studies, Humanities, Cultural Heritage, History, Archaeology and related fields
through a thematic cluster of European Research Infrastructures, integrating initiatives, e-infrastructures and other world-class infrastructures, and building bridges between
different, although tightly, interrelated fields. PARTHENOS approach to achieve this objective was set through the definition and support of common standards, the coordination
of joint activities, the harmonization of policy definition and implementation, and the development of pooled services and of shared solutions to the same problems.
In the framework of Parthenos WorkPackage 4 on Standardisation, aimed to provide support to researchers in using specific standards, activities have been carried out in the
context of complete research scenarios, created by domain experts and designed to be displayed within the Standardization Survival Kit web application, visible at
(https://www.parthenos-project.eu/portal/ssk-2); (http://ssk.huma-num.fr/#/scenarios) 
The final report of this work on the definition of the Standardization Survival Kit (SSK) has been published in Zenodo:  [Romary, Laurent, Riondet, Charles, Tadjou, Lionel, Sotiropoulou, Sophia, & Seillier, Dorian. (2019). PARTHENOS D4.4 Report on Standardization – Final]. (see also Annex 1- Heritage Science specific activities) (https://doi.org/10.5281/zenodo.2607014)

### Parthenos Heritage Science standardization activities

In the domain of Heritage Science standardization is not well-advanced and there is a rather limited number of procedures or protocols that are carried out following an
approved standard workflow. This is explained by the fact that institutions or domain experts follow well defined protocols, either based on institution tradition or expert’s
own experience as well as on generally adopted best practices, which are, however, often designed for specific ends or adapted to available instrumentation or case specific
conditions in which the analytical campaign is carried out. However, the impact of standard procedures in upgrading the safety of users/operators and objects, the performance
of the methods, the quality, reliability of the results is well recognised.
Further, there is a common will to obtain effective interoperability between different Heritage Science communities and integration of inter/cross/trans disciplinary
information; to this end, rules and standards need to be established for the documentation of data produced from the different communities. The development and adoption of
“universal” protocols and standards are intended as reference framework to generate valuable information and suitable metadata to be stored, accessed, queried, shared and
reused among the institutions, scientists and conservation professionals in various contexts and research scenarios. Exchange and creation of new knowledge across disciplines,
actions, research and services put in central focus the efficient interoperability of data (Wilkinson et al. 2016).

The main inhibitors for the interoperability of data across institutions, domain experts and disciplines is the incompatibility of data formats, heterogeneity of data
representation (metadata schemas) and lack of common interdisciplinary understanding/interpretation of the data. During this “pre-standardization” phase, documents describing
established analytical protocols and best practices need to be shared, assessed and be widely accepted through consensus among experts in the field of Heritage Science.

In this context, the use of the SSK platform was intended, in Parthenos project, to provide a forum for domain experts to gather best practices, exchange and agree on
specifications and criteria to be applied consistently towards standardization procedures. On the same time, the SSK platform supports educational purposes disseminating 
scenarios of research for scientists and professionals new in the field or in the use of a specific method, in particular.
A synchronized, equally major effort was put towards the outline of metadata schemas that will enable interoperability of data produced and related information obtained
through standard protocols. 

The scope of this task was to generate a common general scheme of documentation and metadata structure adaptable to be specific of the different analytical protocols and
procedures but retaining a standard/template outline enabling exchange of information in a proper way. More precisely, SSK scenarios that describe in detail the steps to 
follow in the application and documentation of specific analytical protocols for the in situ characterization of materials on heritage objects have been enriched with the
related structure of metadata for data representation. Furthermore, the metadata have been mapped in CIDOC-CRM (and compatible models) as a common and extensible semantic
framework to formulate relevant information on the analytical protocols, related projects, analytical or conservation campaigns and heritage objects involved in a structured
manner compatible for information systems . CIDOC-CRM has been used as a semantic reference model which reinforces compatibility and enables exchange of digital information
resources produced and stored in different management systems.

#### References
[CIDOC CRM (ISO 21127:2006)] (http://cidoc-crm.org) Core model + domain-specific extensions as [CRMsci Scientific observation information] - (http://cidoc-crm.org/crmsci); [CMRdig Provenance metadata for digital objects] (http://cidoc-crm.org/crmdig)
Wilkinson, Mark D., Michel Dumontier, IJsbrand Jan Aalbersberg, et al., 2016. "The FAIR Guiding Principles for Scientific Data Management and Stewardship" 
in Scientific Data 3: 160018.
