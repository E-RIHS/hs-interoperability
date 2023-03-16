# Vocabulary Managment System Requirements

In large part based upon Monica Monachini, Taina Jääskeläinen, Dieter Van Uytvanck, Iulianna Van der Lek, Daan Broeder and Yoann Moranville, MS8 Choice of Vocabulary Publication platform for SSHOC, version 1.0 (Zenodo: 2021). DOI: https://doi.org/10.5281/zenodo.5181389 

## Infrastructure 
- [ ] Data model:  capable of implementing all SKOS elements (including SKOS-XL), including synonyms (ideally distinguishing between usable and retrieval-only), related concepts, node labels, and concept schemes 
- [ ] Data structure: polyhierarchical 
- [ ] Ability to add ad-hoc fields to any concept schema to hold additional (typable) data 
- [ ] ? Multilingual, supporting translation management 
   - [ ] System remembers language choice when translating / editing 
   - [ ] Original text visible when translating 
   - [ ] Other languages easily visible when translating 
- [ ] Architecture: browser-based 
- [ ] Version control, including ability to map to an entity at any previous version or define the current version, and audit trail of all labels / concepts / concept schemes 
- [ ] Records provenance, i.e. who is responsible for changes, with ability to add reason for change 
- [ ] GUIs for administration, editing / translating, viewing 
- [ ] Granular role-based user permissions (embodying view / edit / create / delete) assignable to each user concept scheme-by-concept scheme and language-by-language (if implementing multilinguality) 
- [ ] ? Integrates with Gallery single sign on 
- [ ] Integrates with Gallery PID infrastructure, assigning PIDS to labels / concepts / hierarchies  

## Viewing (browsing) 

- [ ] Can show all data and metadata at all levels, including PIDs
- [ ] Tree view
- [ ] Browse in any given language
- [ ] Facet browsing, including: 
   - [ ] By concept scheme 
   - [ ] By external source 
   - [ ] By external link (e.g. 'all labels with AAT mapping') 
   - [ ] By language (if implementing multilinguality) 
- [ ] Label and concept search 
   - [ ] Organise results returned (relevance / alphabetically, etc.) 
   - [ ] Auto-complete 
   - [ ] Indexes all labels, including non-preferred and hidden 
   - [ ] Shows hierarchy in search results, including expanded hierarchy  
- [ ] View raw data serialised as … 

## Editing 

- [ ] From SSHOC MS8: Management of labels should provide information about status, language, unique URI type identifier [PID], notes of different types associated with labels, equivalence relations between concepts, hierarchical and associative relations between concepts, e.g. hierarchical relationships (narrower, broader), association relationships (related labels), semantic relationships (synonyms), authorised semantic relationships (one of the synonyms is identified as Preferred Label, PT), translations (and what elements are translated)
- [ ] Ability to define a preferred language
- [ ] Drag-and-drop movement / copying of concepts
- [ ] Multiple definable sort options for concepts within hierarchies:
   - [ ] Manually defined
   - [ ] Alphanumeric
- [ ] Identify candidate labels with approval workflow; ability to approve all children / descendants at once
- [ ] ? ((Semi-)automated) alignment with external vocabularies
- [ ] Define sub-sets of vocabularies for use in particular contexts, either particular facet(s) or individual concepts identified manually / by pre-defined search

## Interoperability 

- [ ] Import SKOS serialised as …
- [ ] Export label / concept / vocabulary as SKOS serialised as …
- [ ] Export versioning and other metadata for labels / concepts / vocabularies as DC?
- [ ] REST API / CIIM integration
- [ ] Meets standards for FAIR data

## Controlled Lists

- [ ] In addition to the above direct vocabulary management and structural requirements the final solution will have to be able to manage controlled lists populated with a subset of terms managed in the vocabulary. This may be achieved as part of the slected vocabulary system or may need to be delivered by an additional system.
