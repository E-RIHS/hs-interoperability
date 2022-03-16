## NFFA EUROPE Pilot / MDMC Helmholtz SEM metadata schema

> Many groups within the broad field of Materials Science are already developing metadata schemas and ontologies, driven by their individual organizational
> goals and guided by the open and FAIR data initiatives (e.g., EOSC, Horizon 2020, Horizon Europe, Turning FAIR into reality). However,
> to promote interoperability, a harmonization approach to find a common description of the data coming from the measurements needs to be developed and
> should be adopted as far as possible.
> Motivated by this, we started a coordination effort between the two projects
> we are directly involved in: the NFFA (Nanoscience Foundries and Fine Analysis)
> EUROPE Pilot (NEP) and the Joint Lab “Integrated Model and Data
> Driven Materials Characterization” (MDMC) of the Helmholtz Association.
> Our final objective is to describe the entire workflow of an experimental project,
> providing rich metadata to make data interoperable. This is an incremental
> process; as a first use case, we developed a metadata schema to describe Scanning
> Electron Microscopy (SEM) measurements. This schema is aiming to become a
> de-facto standard for SEM and to pave the way towards further extension to
> other electron microscopy techniques.

PDF in this folder describes the schema in a general way, and discusses it use in Nexus files. (Does any SEM(-EDX) software packages support this format?)

Schema in XSD format and examples on: https://msc.datamanager.kit.edu/msc/m110


_Comment from Wim Fremout:_

This metadata schema allows for an (too?) extensive description of SEM and FIB experiments, but lacks (in my opinion) detail in detector parameters, and in particular for EDX experiments. Might provide a good basis, but requires evaluation by other labs.