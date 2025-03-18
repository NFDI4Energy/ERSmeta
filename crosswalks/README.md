# Crosswalks

Within this folder, crosswalks to different existing metadata schemas are provided.

## General
For each crosswalk, we provide a csv file with the following columns:
* ERSmeta URI: URI of the property in ERSmeta
* ERSmeta Property: name of the property in ERSmeta
* ERSmeta Type: type of the property in ERSmeta
* ERSmeta Description: description of the property in ERSmeta
* Other schema URI: URI of the property in the other schema
* Other schema Property: name of the property in the other schema
* Other schema Type: type of the property in the other schema
* Other schema Description: description of the property in the other schema

For some schemas, some columns may not exist because the information is not provided by the schema.

## Related schemas

### CodeMeta
[CodeMeta](https://codemeta.github.io) is a metadata schema to generally describe research software. Version 3.0 of CodeMeta is used for the crosswalk.

### CFF
[CFF](https://github.com/citation-file-format/citation-file-format/tree/main) is a schema to provide plaintext metadata for software and datasets. Version 1.2 of CFF is used for the crosswalk.

### Software Description Ontology
The [Software Description Ontology](https://knowledgecaptureanddiscovery.github.io/SoftwareDescriptionOntology/release/1.9.0/index-en.html) is an ontology to describe research software. Version 1.9 of the SoftwareDescriptionOntology is used for the crosswalk.

### DataDesc
[DataDesc](https://github.com/FZJ-IEK3-VSA/DataDesc/tree/main) is metadata schema for software focusing on the aspects of interfaces. Version 1.1. of DataDesc is used for the crosswalk.

### Open Energy Platform Framework Factsheets (OEPFF)
The [Open Energy Platform](https://openenergyplatform.org/) includes [factsheets on frameworks](https://openenergyplatform.org/factsheets/frameworks/). These factsheets are based on a non-formalized metadata schema.
A crosswalk to the current version (17.03.2025) of these framework factsheets is provided.
