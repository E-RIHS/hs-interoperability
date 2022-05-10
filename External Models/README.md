
# External Conceptual Models and Ontologies

Please add to this list any external models that are being used in this work:

```The format for this list is still to be defined - we need names and links - but it would also be useful to have comments and links to which local models these external models are used in.```

## CIDOC CRM
https://www.cidoc-crm.org/

CIDOC CRM a high-level ontology for the humanities that is increasingly used for heritage science data. The “CRM” stands for “conceptual reference system”. It sees the world as a series of events, i.e. meetings of people, ideas and objects, which interact with each other in limited areas of space, time and periods, and bring about noteworthy changes. CIDOC CRM consists of **classes** such as *Actor* (which is a person or a group) or *Activity* (which is an event that is intentionally carried out by an Actor, as opposed to e.g., a volcanic eruption) and **properties** that connect these classes: for example, the property *carried out by* connects an Activity with an Actor, as in “the painting of the Sistine Chapel *carried out by* Michaelangelo Buonaroti”. 

It employs a strict bottom-up approach, which means it is always based on real data to be modelled. For example, when the concept of acqusition was introduced early on in the development of the CIDOC CRM, a use case was the acquisition of an object by a museum. This explains the restriction to physical things, i.e. Acquisition cannot be used to describe for example, the copyright of a song.

Each class or property has a number and a name, for example *E8 Acquisition* or *P24 transferred title of*, which names the *E18 Physical Thing* that is being acquired. The name should give a hint about its meaning, but the correct way to understand the class or property is to read the **scope note** that explains which things belong to it, and to look at examples. It is a common mistake to use classes and properties whose names sound as if they describe what one is looking for but where the scope note makes clear that they don’t. For example, when a property is called consists of, it is not clear from the name whether it applies to things or periods.

Classes and properties each form a **hierarchy** where more general classes and properties are higher up and more specific ones are further down. For example, *E96 Purchase* is a **subclass** of *E8 Acquisition* that only applies when money changes hands in the acquisition. *P11 had participant*, which connects E5 Event with an E39 Actor, has a **subproperty** *P14 carried out by*, which only applies when the Event is in fact an Activity and the Actor actively participates in it. As a general rule when using CIDOC CRM, be as specific as you can, but don’t hesitate to use a less specific class or property that is sure to fit. For example, if it is not clear whether an Actor actively participated in an Activity or was “just there”, using the more general *P11 had participant* is fine. 

When *P14 carried out by* connects an E7 Activity with an E39 Actor, then the E7 Activity is called the **domain** and the E39 Actor the **range**. The domain and range are comparable to the subject and object in a simple “subject verb object” sentence. Virtually all properties have **inverses** where the domain and range are swapped. For example *P14 carried out by* has the inverse property *P14i performed*, which connects the E39 Actor with the E7 Activity.

All statements consist of one or more simple “subject verb object” sentences, where the object of one sentence is the subject of the next sentence. For example, an architrave is a lintel that rests on the capitals of columns. the statement “the architrave dates probably from the early 3rd century CE” looks like this:

```
E22 Human-Made Object "Architrave"
	P108i was produced by E12 Production
		P4 has time-span E52 Time-Span
			P86 falls within E52 Time-Span "probably early 3rd century CE"
```

actually consists of several “subject verb object” sentences:


| subject | verb | object |
| --- | --- | --- |
| E22 Human-Made Object "Architrave" | P108i was produced by | E12 Production (of the architrave) |
| E12 Production (of the architrave) | P4 has time-span |E52 Time-Span (denoting the exact time, which is unknown) |
| E52 Time-Span (denoting the exact time, which is unknown) | P86 falls within | E52 Time-Span "probably early 3rd century CE" |

Since CIDOC CRM is event-based, another way of stating exactly the same information would be to start at the production event of the architrave:

```
E12 Production
	P4 has time-span E52 Time-Span
		P86 falls within E52 Time-Span "probably early 3rd century CE"
	P108 has produced E22 Human-Made Object "Architrave"
```

This leads to the same “subject verb object” sentences, only in different order and with *P108 has produced* instead of the inverse *P108i was produced by*: 

| subject | verb | object |
| --- | --- | --- |
| E12 Production (of the architrave) | P4 has time-span |E52 Time-Span (denoting the exact time, which is unknown) |
| E52 Time-Span (denoting the exact time, which is unknown) | P86 falls within | E52 Time-Span "probably early 3rd century CE" |
| E12 Production (of the architrave) | P108 has produced | E22 Human-Made Object "Architrave" |


## HESCIDA (KIK/IRPA)

HESCIDA is an E-RIHS.be project lead by KIK-IRPA that aims to create a heritage science knowledge base with art historical, conservation/restoration and material data. 
It builds on the existing BALaT portal hat contains a unique collection of over 850 000 photos of Belgian heritage, an authority list of persons & institutions, and the library catalogue. 
A vast treasure of archives remained however undisclosed. Almost 20 000 intervention files since the inception of KIK/IRPA contain evidence of a rich past and present in the research and 
treatment of numerous heritage objects: condition, conservation, restoration and laboratory reports, detailed images taken during restoration, samples, analytical data... HESCIDA will
provide tools to document this data and to disclose it in BALaT and a repository.

The HESCIDA stack will consist of several tools. The art-historical data, persons & institutions database and library collection are managed by a commercial collection management system,
currently Adlib and in the near future Axiell Collections. Images are served by a IIIF-server and will by managed by a bespoke digital assets management system (DAMS). All other datasets 
are being collected in a centralised file archive, and will be documented with Metahub. This bespoke metadata collector platform will allow researchers to manage and document intervention 
files, reports, analytical datasets, samples and sample collections. In doing so, links will be made between those enitities and with the entities stored in the other data sources.

Due to the widely differing metadata that needs to be stored in Metahub and the need to create a user-friendly environment for the researchers, a versatile mechanism is implemented in 
Metahub: 4 basic models are created: projects (including intervention files), datasets (reports, scientific imaging, analytical data), samples and sample collections. These 4 models 
only contain the most rudimentary metadata that is required for the proper functioning of the software. Each of those basic models can be extended to cater for specific needs in two tiers.
The first tier, categories, are meant to define universal metadata schemas, while the second tier, templates, are used to define very specific schemas.

An example of a category is a metadata schema for Raman spectroscopy. Many heritage science institutions have one or more systems, in different set-ups. Using the [category schema for Raman spectroscopy](https://github.com/E-RIHS/hs-interoperability/blob/main/External%20Models/HESCIDA%20(KIK-IRPA)/raman.json), it should be able to document any Raman spectrum, whereever it was created, whatever instrument was used. 
This scheme does not arise out of nowhere, but is heavily influenced by the [metadata schema](http://irug.org/uploads/documentation/irug-jcamp-dx-revised-white-paper-text-only-with-2b-version-1-26-sept-2013.pdf) 
developed by the [IRUG](http://irug.org/) community. The IRUG metadata is part of the specification to store data and metadata in the open JCAMP-DX format. The focus of IRUG, however, is
on reference samples, and is not well adapted for more complex sample types. Sample metadata is not included in the HESCIDA Raman metadata schema, but documented in a separate, linked
entity.

An example of a template is a [metadata schema for a Raman spectroscopy experiment, conducted with the Renishaw InVia, equiped with a NIR 785nm laser](https://github.com/E-RIHS/hs-interoperability/blob/main/External%20Models/HESCIDA%20(KIK-IRPA)/raman_invia785.json). The template metadata schema contains a specific set-up at KIK/IRPA, with many fields having precise predefined values. This eases the researcher in 
documenting the experiments.

Currently, the following metadata schemas are uploaded into the HESCIDA subfolder
- raman.json: generic metadata schema for Raman spectroscopy experiments
	- raman_invia785.json: specific schema for an often used set-up at KIK/IRPA
- dendro.json: generic metadata schema for dendrochronology analysis
	- dendro_kikirpa.json: specific schema for dendrochronology at KIK/IRPA
- drms.json: generic metadata schema for drilling resistance measurements
(more will be added)

Note: these are draft schemas, and we welcome comments and contributions