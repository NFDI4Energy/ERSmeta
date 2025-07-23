# ERSmeta: A Metadata schema to describe energy research software

ERSmeta is a metadata schema designed to facilitate the discovery, sharing, and reuse of energy research software. The schema provides a standardized way to describe the metadata associated with energy research software, including its purpose, functionality, and usage.

ERSmeta is based on [CodeMeta](https://codemeta.github.io) and also reuses elements from [metadata4ing](http://w3id.org/nfdi4ing/metadata4ing#), [the open energy ontology (OEO)](	http://openenergy-platform.org/ontology/), [the Software Description Ontology](https://w3id.org/okn/o/sd), and [ontosoft](http://ontosoft.org/software#).

## Provided Formats
ERSmeta is provided in two formats:

#### SHACL
A **SHACL formalization** can be found  as [turtle file](schema/ERSmeta.ttl). It contains all constrains of the metadata schema.

#### JSON-LD
The metadata schema is also provided as **JSON/JSON-LD**. It consists of the JSON schema and the context file.
The context for JSON-LD can be found in [this file](schema/ersmeta.jsonld). It maps all elements to semantic web items.

The JSON schema can be found in [this file](schema/ersmeta_schema.json). This schema includes less constrains than the SHACL formalization since some constrains can not be formalized in JSON, e.g., the limitation of a value of element to a certain ontology class.

## Documentation
A **general description** of the metadata schema can be found on its [documentation website](https://nfdi4energy.github.io/ERSmeta/). The documentation is automatically build from the SHACL formalization.
Also, a [description of all properties](schema/properties_description.csv) and [a description of all used types (and their properties)](schema/type_descriptions.csv) are provided in this repository. In extension to the SHACL formalization, we add three different priority levels to the elements in the description of all properties: mandatory, recommended, and bonus.

## Crosswalks
We created crosswalks to the following metadata schemas:
* [CodeMeta](https://codemeta.github.io)
* [CFF](https://github.com/citation-file-format/citation-file-format/tree/main)
* [Software Description Ontology](https://knowledgecaptureanddiscovery.github.io/SoftwareDescriptionOntology/release/1.9.0/index-en.html
)
* [DataDesc](https://github.com/FZJ-IEK3-VSA/DataDesc/tree/main)
* [Open Energy Platform Framework Factsheets](https://openenergyplatform.org/factsheets/frameworks/add/)

All crosswalks are available in the [subfolder crosswalks](crosswalks).


## Background
Energy research software is defined as "software used in the scientific discovery process for understanding, analyzing, improving, and designing energy systems" by [Ferenz et al. 2023](https://www.inggrid.org/article/id/3837/).

The metadata schema is based on an [extensive requirement analysis](https://eceasst.org/index.php/eceasst/article/view/2594). In this requirement analysis, interviews with around 30 researchers were performed to gather insides which information are relevant for energy researchers when looking for software.



## How you can help
We welcome help to improve the schema and/or its documentation!
Please open up [issues](https://github.com/NFDI4Energy/ERSmeta/issues) or send us a pull request if you have any updates to our schema or crosswalks!

## Hints on Validating Metadata against the Metadata Schema
If you have metadata as RDF or JSON and want to validate it against the schema we recommend the following tools:
* RDF - SHACL validation: https://shacl-playground.zazuko.com/
* JSON - JSON schema validation: https://www.jsonschemavalidator.net/

## Information for Developers
We recommend the following tools for testing and verifying during the development:
* For JSON-LD: https://json-ld.org/playground/


## License
ERSmeta is released under the [CC0 1.0 Universal](https://spdx.org/licenses/CC0-1.0) license.

## Acknowledgments
The authors would like to thank the German Federal Government, the German State Governments, and the Joint Science Conference (GWK) for their funding and support as part of the [NFDI4Energy consortium](https://nfdi4energy.uol.de/). The work was partly funded by the German Research Foundation (DFG) – 501865131 within the German National Research Data Infrastructure ([NFDI](https://www.nfdi.de)).
