# Shared Models - across all activities
Handling and sharing data related to MOLAB, FIXLAB, ARCHLAB or JRA Projects may require specific data models to be considered or developed to ensure that all of the appropriate metadata is recorded in relation to our work, however. There are several parts of the research data life cycle that can rely on common
models for the data to be collected, generated or processed and preserved. Details of these shared models will be included here. Similar models specifically related to the various Techniques used within MOLAB, FIXLAB, ARCHLAB or JRA Projects will be documented in dedicated folders.
<details>
<summary>Project Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.5.tsv">0.5</a>
</summary>
  
## Project Model Details
Relates to models: Object, Actor, Event

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| | 19-10-2023 | J Padfield | [0.6](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.6.tsv) | | Updated model to make use of the new Documentation Statement model, cleaned up and checked it was correct against current overall model |
| :heavy_check_mark: | 28-06-2023 | J Padfield | [0.5](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.5.tsv) | [0.5](https://e-rihs.io/schema/project-v0.5.schema.json) | More detailed model further developed after considering the details required during the project application process used in IPERION-HS. The model has been developed in line with developments of the older schema document so that the two now align again. |
|  | 18-04-2023 | J Padfield | [0.4](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.4.tsv) | | More detailed model developed after considering the details required during the project application process used in IPERION-HS. Within this model, the details of any listed objects, samples, sites, etc., that are being examined are only referenced and will need to be collected or defined in a separate form based on the Simple Object Model. |
| | 28-11-2022 | J Padfield | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.3.tsv) | [0.3](https://e-rihs.io/schema/project-v0.3.schema.json) | A simplification of the model used as the basis of the initial draft JSON schema document |
| | 24-08-2022 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.2.tsv) | - | Update of the model after further discussion and the assessment of the IPERION HS proposal template. |
| | 17-08-2022 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Project%20Model%20-%20V0.1.tsv) | - | Based on task discussions, this is an initial workup of a Project model. The relationships are actually based on CRM properties. The model has been extended to include the notion of the development or versioning of the project through proposal to success or failure. Further work will be required to determine how best to define the Research Questions (ideas that are motivating the project). |
| | <img width=325 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=500 /> |
</details>
<details>
<summary>Service Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20Model%20-%20V0.6.tsv">0.6</a>
</summary>

## Service Model Details

Relates to models: Object, Actor, Equipment, Project
* This includes the concept of a service "Support Activity" as a nested model.

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
|:heavy_check_mark: | 09-03-2023 | J Padfield | [0.6](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20Model%20-%20V0.6.tsv)  | [0.6](https://e-rihs.io/schema/service-v0.6.schema.json) | Small update to add a field to record optional not for profit Access Unit Costs. |
| :heavy_check_mark: | 08-03-2023 | J Padfield | [0.5](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20Model%20-%20V0.5.tsv)  | [0.5](https://e-rihs.io/schema/service-v0.5.schema.json) | Initially an update of model 0.3 to match schema 0.4, but some differences still need to be resolved in relation to the need for a specific service bibliography and a few other minor differences. |
|:heavy_check_mark: | 08-03-2023 | J Padfield |  | [0.4](https://e-rihs.io/schema/service-v0.4.schema.json) | Formatting updates, added some controlled lists, and checked support activity sub-model. |
|:heavy_check_mark: | 03-02-2023 | J Padfield | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20Model%20-%20V0.3.tsv) | [0.3](https://e-rihs.io/schema/service-v0.3.schema.json) | This model has been updated based on the concept of a Record, which was used to define Tools and services to be listed under E-RIHS.io - a few fields have had some additional examples added - but new metadata fields were also added - the concept of Administration fields was also introduced. |
| :heavy_check_mark: | 12-12-2022 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20Model%20-%20V0.2.tsv) | [0.2](https://e-rihs.io/schema/service-v0.2.schema.json) | This model has been updated based on a service form discussed in an E-RIHS IP T3.4 meeting. |
| :heavy_check_mark: | 28-11-2022 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20Model%20-%20V0.1.tsv) | [0.1](https://e-rihs.io/schema/service-v0.1.schema.json) | This model represents the core metadata fields required to specifically describe a given Service. Full metadata details of the actual work carried out would need to also include details of related models, such as people, and equipment. |
| | 24-11-2021 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Service%20and%20Application%20Simple%20Model%20-%20V0.1.tsv) |  | Original more broad, initial Service and Application model. |
| | <img width=325 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=500 /> |
</details>
<details>
<summary>Actor Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Actor%20Model%20-%20V0.1.tsv">0.1</a>
</summary>

## Actor Model Details

Relates to models: Service, Project, Examination
* To keep things simple the Actor model has been split into two related overlapping Schema: Person and Orginisation

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| :heavy_check_mark: | 18-01-2023 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Actor%20Model%20-%20V0.1.tsv) | [0.2O](https://e-rihs.io/schema/organisation-v0.2.schema.json), [0.2P](https://e-rihs.io/schema/person-v0.2.schema.json) | The two schema represent two versions of the Actor model, one for Organisations (O) and one for Person (P) |
| | <img width=325 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=500 /> |
</details>

<details>
<summary>Documentation Statement Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Documentation%20Statement%20Model%20-%20V0.1.tsv">0.1</a>
</summary>

## Documentation Statement Model Details

Relates to models: Service, Project

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| | 19-10-2023 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Documentation%20Statement%20Model%20-%20V0.1.tsv) | | This new model has been created as a template for a range of different situations where one of more statements need to be made about a particular entity. |
| | <img width=475 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=400 /> |
</details>

<details>
<summary>Method Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Method%20Model%20-%20V0.1.tsv">0.1</a>
</summary>

## Method & Standard Method Model Details

Relates to models: Service, Project

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| | 19-10-2023 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Method%20Model%20-%20V0.1.tsv) | | This new model has been created as a template for a range of method or setup descriptions - it allows for methods based on a series of statements and or a selection of the defined method parameters - It is also structured to allow the notion of the a deafule Standard Method, which is is then used as the basis for a unique derivative method applied to a given process.|
| | <img width=475 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=400 /> |
</details>


<details>
<summary>Support Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Support%20Model%20-%20V0.2.tsv">0.2</a>
</summary>

## Support Model Details

Relates to models: Service, Actor, Project

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
|:heavy_check_mark: | 08-03-2023 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Support%20Model%20-%20V0.2.tsv) |[0.4<sup>*</sup>](https://e-rihs.io/schema/service-v0.4.schema.json) | This model has been simplified as many metadata fields as now covered by the Actor model - <sup>*</sup>Please note this model is actually included as a sub-model in the Services schema. |
| | 11-01-2023 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Support%20Model%20-%20V0.1.tsv) | | This model is an initial draft exploring the notion of entities that support services. It has been described as Funding Programme before. It began with the idea of defining the source of funding for a given service, but it has been discussed that different types of support might be provided along with multiple instances so a more flexible relationship is required. Also, actual institutions/organisations can be defined separately as types of Actors so they can be linked or referenced here rather than being defined again. |
| | <img width=475 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=400 /> |
</details>
<details>
<summary>Research Activity Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Activity%20Model%20-%20V0.6.tsv">0.6</a>
</summary>

## Research Activity Model Details(was Examination Model)

Relates to models: Project, Object, Actor, Event

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| | 19-10-2023 | J Padfield | [0.6](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Activity%20Model%20-%20V0.6.tsv) | | General updates and updated to exploit the new Documentation statement and Method models |
| | 11-10-2023 | All | [0.5](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Activity%20Model%20-%20V0.5.tsv) | | Confirmed measurement capture and added in interpretation capture" |
| | 04-10-2023 | J Padfield | [0.4](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Activity%20Model%20-%20V0.4.tsv) | | Further extended to improve measurement description, classification and define place to list measurement parameters. Additionally the fields required to add one of more optionally illustrated activity documentation statements has been added." |
| | 30-08-2023 | J Padfield | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Activity%20Model%20-%20V0.3.tsv) | | Further clarifcation of the model including the oiption to have multiple "measurements" within a single "Object Examination" |
| | 23-08-2023 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Activity%20Model%20-%20V0.2.tsv) | | The examination model has been extended to cover a more general research activity which can be an examination but could also be a data processing activity. The Tooltips in the model may well be out of date or need adding |
| | 15-09-2022 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Examination%20Simple%20Model%20-%20V0.1.tsv) | | This the initial draft model created based on previous discussions related to techniques and equipment. It relates tot he examination of object or archives, further thought is needed to assess what metadata will be useful when considering Archive Examinations. |
| | <img width=475 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=400 /> |
</details>
<details>
<summary>Research Focus Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Focus%20Model%20-%20V0.4.tsv">0.4</a>
</summary>

## Research Focus Model Details (was Object Model)

Relates to models: Actor, Event

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| | 19-10-2023 | J Padfield | [0.4](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Research%20Focus%20Model%20-%20V0.4.tsv) | | Converted Object model tot he broader Research Focus model - Covering Objects, Samples, Archives, or Datasets - It is anticipated that Datasets would also come with it standard DOI like metadata that would replicate some of the fields included. |
| | 18-04-2023 | J Padfield | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Object%20Simple%20Model%20-%20V0.3.tsv) | | DRAFT Tidying up the model, checking its use in relation to the Projects model and the broad definition of Focuses of Study |
| | 21-10-2021 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Object%20Simple%20Model%20-%20V0.2.tsv) | | Creation of V0.2, added in formatting to improve the clarity of the model and along with increased details of the included fields |
| | 20-10-2021 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Object%20Simple%20Model%20-%20V0.1.tsv) | | Creation of the first draft example of a simple object model, based on the Parthenos spreadsheet|
| | <img width=325 /> |<img width=175 /> | <img width=60 /> | <img width=60 /> | <img width=500 /> |
</details>
<details>
<summary>Technique Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Technique%20Model%20-%20V0.4.tsv">0.4</a>
</summary>

## Technique Model Details

Relates to models: Object, Measurement

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| :heavy_check_mark: | 31-05-2023 | All | [0.4](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Technique%20Model%20-%20V0.4.tsv) | [0.4](https://e-rihs.io/schema/technique-v0.4.schema.json) | Simplified model - extended SKOS type description. |
|| 23-06-2022 | J Padfield | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Technique%20Model%20-%20V0.3.tsv)|| Simplified to a general technique rather than specific details related to equipment etc.|
|| 24-11-2021 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Technique%20Model%20-%20V0.2.tsv) || First generic draft - designed to cover a range of different techniques - more targeted models may be required. |
|| 02-11-2021 | S Sotiropoulou | 0.1 | - | Initial draft |
|| <img width=140/> |<img width=125/> | <img width=60/> | <img width=60/> | |
</details>
<details>
<summary>Tool Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Tool%20Model%20-%20V0.4.tsv">0.4</a>
</summary>

## Tool Model Details (Was Equipment)

Relates to models: Object, Measurement
* Changed to a Tool model to include the concept of software and hardware
* The idea of a tool is just generic and, as they can be nested, this model can also cover the broader idea of Facilities and Platforms of equipment and software.
* Please note when details of people need to be included in relation to those hosting or running a given tool are required, then one needs to consider the Service model

| | Date  | Author | Model | Schema | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| | 20/10/23 | J Padfield | [0.4](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Tool%20Model%20-%20V0.4.tsv)| | Updated to be more consistant with others and to make use of the Method, Documentation Statement and Research Activitiy models. |
| :heavy_check_mark: | 19/07/23 | Joe & Wim | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Tool%20Model%20-%20V0.3.tsv)| [0.3E](https://e-rihs.io/schema/equipment-v0.3.schema.json), [0.3S](https://e-rihs.io/schema/software-v0.3.schema.json) | Moved to the generic Tool concept rather than just equipment and updated model slightly to match the schema. Two schemas have been produced for this model, one for Equipment and one for Software. |
|| 14/06/23 | All | [0.3](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Equipment%20Model%20-%20V0.3.tsv)| - | Split the notion of Equipment into Equipment(E)/Software(S) under the notion of Tools. Also extended the model slightly. |
|| 21/03/23 | J Padfield | [0.2](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Equipment%20Model%20-%20V0.2.tsv)| - | Extended slightly but also made more generic. |
|| 23/06/22 | J Padfield | [0.1](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Equipment%20Model%20-%20V0.1.tsv)| - | Simplified draft for a general piece of equipment etc. |
|| <img width=140/> |<img width=125/> | <img width=60/> | <img width=60/> | |
</details>
<details>
<summary>Measurement Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Measurement%20Simple%20Model%20-%20V0.1.tsv">0.1</a>
</summary>

## Measurement Model Details

Relates to models: Access, Project, Technique, Service

| Date  | Author | Version | Link | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| 10-11-2021 | S Sotiropoulou | 0.1 |[LINK](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Measurement%20Simple%20Model%20-%20V0.1.tsv)
| <img width=110/> |<img width=90/> | <img width=60/> | <img width=60/> | |
</details>
<details>
<summary>Dimension Model: 
<a href="https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Dimension%20Model%20-%20V0.1.tsv">0.1</a>
</summary>

## Dimension Model Details

Relates to models: Access, Project, Technique, Service

| Date  | Author | Version | Link | Comment |
| :-----------: | :-----------: | :-----------: | :-----------: | ----------- |
| 16-03-2023 | J Padfield | 0.1 |[LINK](https://national-gallery.github.io/dynamic-modelling/?url=https://raw.githubusercontent.com/E-RIHS/hs-interoperability/main/Shared%20Models/Dimension%20Model%20-%20V0.1.tsv)
| <img width=110/> |<img width=90/> | <img width=60/> | <img width=60/> | |
</details>
