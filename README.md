[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7221156.svg)](https://doi.org/10.5281/zenodo.7221156)

# Heritage Science Interoperability
Ongoing work in relation to the IPERION-HS project and the related E-RIHS IP project, to explore methods to improve interoperability across Heritage Science data. At this stage we are working to define the required meta and para-data needed to ensure that data gathered during technical examinations can be FAIR. To achieve this we are currently working on a number of steps:

## Current Development
Comments and descriptions still to be added
1. **Define discrete Re-usable data modules:** This work is currently ongoing - see [here](./Shared%20Models/README.md)
2. **Map the relationships between data modules:** This work is currently ongoing - see [here](./Model%20Relationships/README.md)
3. **Define the core meta data fields needed for each data module:** Work related to the development of vocabularies will brought together [here](https://vocab.e-rihs.io/)
4. **Define the generic JSON schema template for each data module:**
5. **Define the specific versions of these JSON schema templates:** The JSON schema are being organised [here](https://e-rihs.io/schema/)
6. **Define initial storage for gathered metadata:** The core storage structure for the E-RIHS metadata will make use of the [Cordra](https://www.cordra.org/) software and the administration interface will be hosted [here](https://data.e-rihs.io/)
7. **Begin to gather test metadata:** on going ....

## Future Work
1. **Define production data storage and search options:**
2. **Integrate existing data into the process of gathering new related data:**
3. **Design improved GUIs for customised data entry**

## Related Tools and Services
Here are some of the tools being used or considered as part of this work:
### The Dynamic Modeller
An interactive live modelling system which can automatically convert simple tab separated triples into graphical models using the [mermaid library](https://mermaid-js.github.io/mermaid). 
- Code: https://github.com/jpadfield/dynamic-modelling
- Live tool: https://research.ng-london.org.uk/modelling/
- https://github.com/bumbu/svg-pan-zoom also being considered for presentation of models.

### Json Form Editors
Both of these systems are currently being used to test the auto generation of the forms from agreed JSON schema templates.
- https://bytes.kikirpa.be/form-generator/ (https://github.com/KIKIRPA/form-generator)
- https://github.com/json-editor/json-editor
The actual production forms (for administration purposes) will be based on:
- https://cordra.org/

### Json Validators
- https://www.jsonschemavalidator.net/
- https://jsonlint.com/

## Acknowledgement
This project was developed and tested as part of the work of the following projects:

### The H2020 [IPERION-HS](https://www.iperionhs.eu/) project
[<img height="64px" src="https://github.com/jpadfield/simple-modelling/blob/master/docs/graphics/IPERION-HS%20Logo.png" alt="IPERION-HS">](https://www.iperionhs.eu/)
###### [IPERION-HS has received funding from the European Union’s Horizon 2020 call H2020-INFRAIA-2019-1, under GA 871034](https://cordis.europa.eu/project/id/871034)
### The Horizon Europe [E-RIHS IP](https://www.e-rihs.eu/the-project/) project
[<img height="64px" src="https://e-rihs.io/graphics/e-rihs-eric-logo_ai.png" alt="E-RIHS IP Logo">](https://www.iperionhs.eu/)<br/>
###### [E-RIHS IP has received funding from the European Union’s Horizon Europe call HORIZON-INFRA-2021-DEV-02, Grant Agreement n.101079148.](https://cordis.europa.eu/project/id/101079148)
