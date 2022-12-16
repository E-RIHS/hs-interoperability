# HMSA

The MSA / MAS / AMAS HyperDimensional Data File (HMSA, for short) is intended to be a common format to permit the exchange of hyper-dimensional microscopy and microanalytical data between different software applications. See also the [Techniques section on SEM-EDS](https://github.com/E-RIHS/hs-interoperability/tree/main/Technique/SEM-EDS) in this github repository, where open file formats and metadata schemas are being discussed. Here, on the other hand, the focus is on building a metadata schema that may facilitate the integration of SEM-EDS data in DIGILAB.

Draft 1.0 dates from 2019 and is submitted to become an official ISO standard.

Currently, there is not much software support, with the exception of [HyperSpy](https://hyperspy.org). It is however expected that this format is going to become the default interoperable format for hyperdimensional microscopy and microanalytical datasets. Because of this, and because there seem to be no viable alternatives, it seems logical that the HS community should embrace this format. We should try to, 
- at the very least, take into account this format for later integration in DIGILAB services
- base our metadata schemas for electron microscopy (and others?) on HMSA
- (if resources are available) develop tools to facilitate the creation of HMSA compliant files and their 

# JSON Schema

JSON Schema is a standard for modelling metadata in a well-defined structure that allows different software applications to understand and integrate the metadata and corresponding data. The metadata are stored in JSON format, which is very straightforward and human readable. JSON is currently by far the most used data exchange format in web technologies because of its simplicity and compact notation.

The HMSA format defines hyperdimensional data in file pairs. The data itself is stored in a simple binary format (.hmsa) and is accompagnied by an XML file (.xml) that contains the metadata in a well-defined structure. XML is an older data exchange format with high verbosity and higher complexity (hence its declining popularity). It has a few features that are not supported in JSON, and only one of those is used in the HMSA draft, namely attributes. However, it is perfectly possible to map the metadata in the two formats.

## hmsa.schema.json

This file contains an early, far from finished draft of the HMSA metadata schema, mapped into a JSON Schema. Because of the comprehensiveness and flexibility of the HMSA specification, the JSON Schema will be very long. Only a small fraction of the HMSA specifications have been mapped.

The general idea of the JSON Schemas that are developed in IPERION-HS, HESCIDA and E-RIHS IP, is to ease the work of the researchers to submit their documented data in a semantical, interoperable and reusable way. For this, the idea exists to use the JSON Schemas to create web forms where the researchers and end-users can describe all different resources, such as experiments, samples, projects...

## developing JSON Schemas

To facilitate the creation the JSON Schemas, we have developed a [small web application](https://bytes.kikirpa.be/form-generator/) in IPERION HS. It allows us to visualise the corresponding web forms for the schemas. (It is for testing purposes only and not intended to be used to fill in real (meta)data). 

Even though the ´hmsa.schema.json´ is far from complete, and because of the comprehensiveness and flexibility of the HMSA metadata, the corresponding web form is already bloated and slow to render. It its current form, many researchers will be put off and fill in the minimal amount of metadata. Very limited metadata is actually required by the HMSA specification, but this contrasts with the need for interoperability.

The primary goal of the JSON files is their ingestion in the DIGILAB tools and not offering web forms. It is possible, and in this case, preferable that the two goals are split. There are a number of possibilities:
- When tools to create and manipulate HMSA files become available, these tools can be used to document the electron microscopy experiments and store them in HMSA format. When uploading the dataset in DIGILAB, the accompagnying XML can be automatically transformed into JSON. This would require a custom made mapping tool in the DIGILAB workflows.
- Simpler JSON Schemas are written for specific electron microscopy set-ups. These schemas would then include only those metadata fields that are required, and often used values can be prefilled. A much simpler web form will then be presented to the researchers. Afterwards, the metadata can be mapped to XML, generating a HMSA compatible file pair, that can be deposited in repositories.

Many variants and intermediate solutions are possible. __It goes without saying that user-friendliness is paramount, along with the goal of complying with the standards used in the electron microscopy community, and with the goals of making the data accessible via DIGILAB.__



