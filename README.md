# QualitativeOntology

[cite_start]This README file describes the main results and provides elaboration on the associated paper, "Domain Ontology for Grounded Theory Qualitative Research: Bridging Interpretation and Structure in Digital Humanities"[cite: 1803].

# Domain Ontology for Grounded Theory Qualitative Research

## 1. Overview and Motivation

[cite_start]This computational ontology was developed to formally represent the key artifacts produced during the research processes of the qualitative **Grounded Theory** approach[cite: 1809].

[cite_start]The motivation for this work is to address an epistemological challenge in Digital Humanities: reconciling the interpretive, context-rich methodologies of the social sciences with the structured, formalized approaches of computational ontology engineering[cite: 1808]. [cite_start]The inherent fluidity of Grounded Theory—with its iterative, data-driven emergence of categories and concepts—makes it difficult to balance deep interpretive insight with systematic rigor and effective management of evolving conceptual relationships[cite: 1817, 1819].

## 2. Main Results and Elaboration (from the Paper)

### A. Core Contribution

[cite_start]The ontology provides a foundational framework to facilitate a more structured approach to analyzing and interpreting qualitative data derived from Grounded Theory research[cite: 1811].

* [cite_start]It offers a formal framework for structuring disciplinary knowledge, thereby enhancing the rigor and clarity of Grounded Theory studies without compromising interpretive richness[cite: 1810, 1820].
* [cite_start]Unlike generic classification systems, this ontology is specifically tailored to capture the emergent, relational, and theory-building aspects of qualitative analysis unique to Grounded Theory[cite: 1523].
* [cite_start]It codifies shared vocabularies and semantic relationships to improve interoperability while preserving the contextual specificity essential to humanistic inquiry[cite: 1821].

### B. Ontology Structure and Flow

The ontology models the entire research cycle, from project formulation to final findings, by defining key classes and object properties. The core structure captures the flow from raw data collection to the generation of conceptual findings:

* [cite_start]**Project Formulation:** A `Project` defines a `MethodologicalStrategy` (`definesStrategy` [cite: 1166][cite_start]), which in turn `appliesTechnique` (`Aplica_una_o_varias`)[cite: 1164]. [cite_start]The project also includes a `TheoreticalFramework` (`Tiene_marco_teorico`)[cite: 1184].
* [cite_start]**Data/Record Generation:** A `Technique` (`isApplicationTechnique` [cite: 1174][cite_start]) is applied to a `SubjectOrObject` (`toSubjectObject` [cite: 1174][cite_start]) via a `TechniqueOverSubjectOrObject` (`Relacionado_a_tecnica_subre_sujeto_u_objeto` [cite: 1175]). [cite_start]This application ultimately `generates` (`Genera`) a `Record`[cite: 1169].
    * [cite_start]*Example:* An `Interview` (`Technique`) is applied to a `Subject` (`SubjectOrObject`), resulting in an `InterviewAnswer` (`Record`)[cite: 1683].
* [cite_start]**Interpretation and Categorization:** A `Record` `isInterpreted` (`Se_interpreta`) by an `Interpretation` entity[cite: 1179]. [cite_start]This interpretation is linked to `DescriptiveCategory` (`Tiene_esquema_de_clasificacion_descriptiva`) and generates `Information` (`Relacionado_a_informacion`)[cite: 1174, 1183].
* [cite_start]**Theory Building:** The `Information` is associated with a conclusion reached by the researcher[cite: 1701]. [cite_start]This `Information` is classified by an `AnalyticCategory` (`Tiene_esquema_de_clasificacion_analitica`)[cite: 1181]. [cite_start]The `TheoreticalFramework` also `impacts` (`Impacta`) the descriptive categories[cite: 1169].
* [cite_start]**Flexibility:** A key design principle is the intentional omission of cardinality restrictions on properties to ensure a model that is flexible and adaptable to the dynamic nature of qualitative data and Grounded Theory[cite: 1752, 1753].


### C. Future Work

[cite_start]Future directions for this work include extending the ontology to encompass other qualitative research methodologies and integrating it with other ontologies in the realm of Open Science[cite: 1776].
