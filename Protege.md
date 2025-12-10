# Simple Guide for Using the Ontology in Protégé

The purpose of using this ontology in Protégé is to formally represent and structure the artifacts and relationships from your specific Grounded Theory research project as **Individuals** (instances of the classes defined in the ontology).

### Prerequisites

1.  **Protégé:** Ensure you have the latest version of the free, open-source **Protégé** ontology editor installed (available from [protege.stanford.edu](http://protege.stanford.edu)).
2.  **Ontology File:** Have the `qualitative_ontology.rdf` file ready.

---

### Step 1: Open and Load the Ontology

1.  **Launch Protégé.**
2.  Go to **File** > **Open...**
3.  Navigate to the location of the `qualitative_ontology.rdf` file and select it.
4.  Protégé will load the ontology. You should see the ontology name/URI at the top.

### Step 2: Navigate the Ontology Structure

The main panels you will use are the **Classes** and **Object Properties** tabs.

#### **Classes** Panel

* This panel shows the main concepts (artifacts) in your Grounded Theory research process, organized hierarchically.
* **Key Top-Level Classes to Note:**
    * `Project` (Your research study)
    * `MethodologicalStrategy` (e.g., Grounded Theory)
    * `Technique` (e.g., Interview, Observation)
    * `Record` (The collected data, e.g., InterviewAnswer, FieldNote)
    * `Interpretation` (The act of interpretation)
    * `DescriptiveCategory` (Initial codes/categories)
    * `AnalyticCategory` (Higher-level themes/concepts)

#### **Object Properties** Panel

* This panel shows the relationships (verbs) that connect the Classes (artifacts).
* **Key Properties to Note (Representing the Research Flow):**
    * `definesStrategy`: Connects a `Project` to a `MethodologicalStrategy`.
    * `generates`: Connects a `TechniqueOverSubjectOrObject` to a `Record`.
    * `isInterpreted`: Connects a `Record` to an `Interpretation`.
    * `Tiene_esquema_de_clasificacion_descriptiva` (Has descriptive classification scheme): Links an `Interpretation` to a `DescriptiveCategory`.
    * `Tiene_esquema_de_clasificacion_analitica` (Has analytic classification scheme): Links `Information` to an `AnalyticCategory`.

---

### Step 3: Creating New Research Individuals (Instantiating the Process)

You will model your own research by creating individuals for each class relevant to your study.

1.  **Navigate to the `Individuals by Class` tab.**
2.  **Select a Class** (e.g., `Project`).
3.  Click the **Add Individual** button (usually a green plus sign).
4.  **Name the individual** (e.g., `MyGroundedTheoryStudy`). This individual now represents your specific research project.
5.  **Repeat this process** for other core classes based on your data:
    * Create an individual for `Technique` (e.g., `SemiStructuredInterview`).
    * Create individuals for your collected data under `Record` (e.g., `InterviewTranscript_001`).
    * Create individuals for your codes/themes under `DescriptiveCategory` (e.g., `Code_WorkLifeBalance`) and `AnalyticCategory` (e.g., `Theme_NegotiationOfRoles`).

### Step 4: Defining Relationships (Connecting Individuals)

This is the most critical step—using **Object Properties**
