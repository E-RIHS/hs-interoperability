# SSHOCro

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

## An early description

An early description (taken from the [SSHOC website](https://sshopencloud.eu/sshocro )) was:

`The SSHOC Reference Ontology (SSHOCro) proposes an ontological model and RDF schema to be used as a top-level ontology for organizing knowledge and information found distributed across various primary sources of information in the Social Sciences and Humanities Open Cloud (SSHOC). It provides a semantic interoperability framework for the description of the data life cycle used by Social Science and Humanities researchers.`

## Discussion points

As for heritage science, it remains to be seen how well the Knowledge Workflow steps can capture the similarities and differences between handling physical objects and the digital data that results from examining the physical objects. At the very least it is not straightforward to model the Knowledge Workflow steps. 

Another open question is where the exact boundary between data processing and data interpretation lies. SSHOCro draws the line between descriptive statistics (e.g. calculating a mean value) and inference statistics (e.g. calculating a p-value, which can be used to decide whether a statistical result is likely a real effect or just an artefact that would disappear when looking at more data). Interpretation further includes everything from the decision that a roof must have had a specific shape up to preparing a report for publication.

A central goal of SSHOCro is to model the provenance of data. However, quite often neither the intermediate datasets nor the Knowledge Workflow steps leading to them are documented. This can make modelling the data provenance quite difficult. And even on the level of the ontology itself it is an ongoing discussion as to how the data provenance should be tracked: Is the knowledge about the data provenance encoded in the “follows” properties that connect the Knowledge Activity steps, or is it encoded in the chain of output/input connections between datasets?

