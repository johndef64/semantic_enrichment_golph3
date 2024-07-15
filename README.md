# Semantic Enrichment of GOLPH3 Gene Dataset

## Description

This project aims to enrich genomic and phenotypic datasets extracted from Ensembl's datamart through semantic enhancement techniques. The target dataset focuses on the GOLPH3 gene and includes both genomic and phenotypic data points.

The GOLPH3 gene encodes an adapter essential for the recycling of Golgi glycosylation enzymes involved in the pathway of glycosphingolipid (GLS) production. Overexpression of GOLPH3 leads to chemoresistance in tumor cells ([Rizzo et al.](https://pubmed.ncbi.nlm.nih.gov/33749896/)). This project aims to uncover additional disease pathways in which the GOLPH3 gene may be involved through a knowledge-driven research approach based on disease ontologies.


The phenotypic data within the dataset has been enriched using two disease ontologies: DOID ([Human Disease Ontology](https://bioportal.bioontology.org/ontologies/DOID)) and MONDO ([Mondo Disease Ontology](https://bioportal.bioontology.org/ontologies/MONDO)). An ontology matcher was developed to facilitate this process. This matcher searches for matches within all synonyms of the ontology classes and appends the IRI (Internationalized Resource Identifier) class ID to the original dataset.

The semantic enrichment of the dataset focusing on the GOLPH3 gene involved cross-linking phenotypic data extracted from Ensembl with disease ontology terms using the DOID and MONDO ontologies. This approach enhances data interoperability and adherence to FAIR principles by appending Internationalized Resource Identifier (IRI) class IDs to the dataset, thereby enabling more efficient data integration and retrieval.


### Key Features
- **Semantic Enrichment**: Enriches phenotypic data using Human Disease Ontology (DOID) and Mondo Disease Ontology (MONDO).
- **Ontology Matcher**: Custom-built tool for matching dataset terms with ontology synonyms and appending Internationalized Resource Identifiers (IRIs) for enhanced data linkage.
- **Data Integration**: Facilitates efficient data integration and retrieval through semantic annotations.


### Repository Content
- **Data Extraction Scripts**: Scripts used to extract the genomic and phenotypic dataset from Ensembl's datamart.
- **Ontology Matcher**: Implementation of the matcher for DOID and MONDO.
- **Semantified Dataset**: The resulting dataset with added IRI class IDs for improved interoperability.

### Usage
1. **Clone the Repository**: Clone the repository to access scripts and datasets.
2. **Run Extraction Scripts**: Use the provided scripts to extract and preprocess the dataset (`ontology_matcher.ipynb`).
3. **Execute Ontology Matcher**: Apply the ontology matcher to enrich the dataset with IRI class IDs.

## Methods
We utilized an ontology matcher to align the phenotypic terms present in the dataset with corresponding terms in the DOID and MONDO ontologies. The matcher searched through all synonyms available in the ontology classes to ensure comprehensive matching and appended the IRI class IDs to the dataset.

## Results
The semantic enrichment process yielded improvements in data interoperability and discoverability:

### Matched Terms
Through the ontology matching process, a considerable number of phenotypic terms were successfully matched to disease ontology terms. Specifically, out of the total phenotypic terms present in the dataset, **68%** were matched with DOID terms and **100%** with MONDO terms.

### Ontology Cross-Referencing
The inclusion of IRI class IDs allowed for enhanced cross-referencing between phenotypic data and disease ontology terms. This cross-referencing facilitates seamless integration with other datasets and ontologies, fostering improved data analytics and hypothesis generation.

## Discussion
The successful integration of DOID and MONDO ontologies into the GOLPH3 dataset enhances its usability in bioinformatics research. The semantically enriched dataset now allows researchers to more easily query and draw connections between the GOLPH3 gene and various diseases. This is critical for uncovering new disease pathways and understanding GOLPH3's role in different pathological conditions.

Additionally, the use of IRI class IDs ensures that the dataset is amenable to automated data retrieval systems and interoperable with other ontological resources. This alignment with FAIR principles further underscores the dataset's utility for the broader scientific community.

### Future Work
- **Expand Ontology Support**: Incorporate additional ontologies for broader semantification.
- **Enhance Matching Algorithms**: Develop more sophisticated algorithms for improved matching accuracy.

[Here is a link to the project repository](https://github.com/your-repo)

### Contact
For questions or contributions, please contact [your-email@example.com].
