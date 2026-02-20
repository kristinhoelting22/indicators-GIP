---
editor_options: 
  markdown: 
    wrap: 72
---

# **1.0 Project Overview**

The purpose of this Global Instruction Preamble (GIP) is to guide AI to
identify relevant **variables** from published research studies and
identify a set of **attributes** of each of those variables. Relevant
variables are those that are being used for a management purpose, which
we defined as being used as an **indicator**. We therefore refer to the
variables identified as indicators. For each indicator identified, these
instructions will guide AI to identify a series of attributes in eight
table outputs. The table outputs produced by AI will support our
research team to double check data previously extracted manually by
humans from a set of articles included in a systematic review of
indicators used in fisheries management. The sections of this GIP are
targeted as follows:

| Section \# | Section Title                                             | Primary Purpose / Output Task                                                                                                                                                                         | Key Constraints / Focus                                                                                                                             |
|:-----------------:|:-----------------|:-----------------|:-----------------|
|  **2.0**   | **Instructions for Identifying Relevant Indicators**      | Defines **inclusion criteria** for filtering text into a list of unique indicators.                                                                                                                   | Indicator must be used for a **management purpose** and be **separately detailed** (Name, Definition, or Score).                                    |
|  **3.0**   | **Variable Type Typology**                                | Codes the indicator's data structure at **three distinct points in time** (Pre-scoring, Scoring, Outcome).                                                                                            | Defines **Codes 1-4** (Basic) and **Codes 5-11** (Outcome/Derived), including **Model Output (10)** inheritance.                                    |
|  **4.0**   | **Conceptual Relationship Coding**                        | Synthesizes attributes for Table 6 (**Conceptual Relationship Code**).                                                                                                                                | **Codes 1-7**. Governed by **Constitutive Code Synchronization Rule** (linking sub-variable codes 3, 4, 5 to parent Outcome Types 6, 7, 8, 10, 11). |
|  **5.0**   | **Community Type**                                        | Codes the indicator's **social relevance focus** (Table 7).                                                                                                                                           | **Default Coding Rules** based on conceptual primary categories (e.g., Fishery Governance $\to$ Code 4; Environmental Context $\to$ n/a).           |
|  **6.0**   | **Unit of Observation**                                   | Codes the **scale of raw data assessment/scoring** (Table 7).                                                                                                                                         | Assessment Scale (1-6) must be determined, or apply **"see sub-variables"** rule if the indicator is a derived output.                              |
|  **7.0**   | **Unit of Analysis**                                      | Codes the **scale of final presentation/interpretation** (Table 7).                                                                                                                                   | Aggregation Rules (e.g., Code 4 for averages/totals) applied to the final reported metric.                                                          |
|  **8.0**   | **Indicator Action**                                      | Codes the **study's intended use** of the indicator (Evaluation vs. Development/Testing) (Table 7).                                                                                                   | **Non-Exclusivity Rule:** Codes 1 and 2 may co-occur ("1; 2").                                                                                      |
|  **9.0**   | **Empirical vs Modeled (Data Source 1)**                  | Codes the **data origin** as **Empirical (1)** or **Modelled (2)** (Table 7).                                                                                                                         | **Symmetry Rule:** Must be consistent with Outcome Type Code 10.                                                                                    |
|  **10.0**  | **Primary vs Secondary (Data Source 2)**                  | Codes the **empirical source** as **Primary (1)** or **Secondary (2)** (Table 7).                                                                                                                     | **Exclusion Rule:** Modelled data must be Code 3 (**Statistically derived**).                                                                       |
|  **11.0**  | **Management Purpose Themes**                             | Codes the **overall management use of the indicator** (Table 5).                                                                                                                                      | Selection of a single best-fit theme from the comprehensive Management Purpose Theme typology.                                                      |
|  **12.0**  | **Sustainability Themes**                                 | Codes the **overall study framing** (Table 5).                                                                                                                                                        | Selection of a single best-fit theme from the comprehensive Sustainability Themes typology.                                                         |
|  **13.0**  | **Conceptual Categories**                                 | Provides the **conceptual typologies** (Definitions) and the **procedural steps** for matching the variable/topic concepts.                                                                           | Requires rigorous **Primary --\> Sub-category** mapping.                                                                                            |
|  **14.0**  | **Relationships Within and Between Indicators**           | Provides **all constitutive and predictive relationship mapping rules** for Tables 2, 3, and 4.                                                                                                       | **Constitutive Symmetry, Link Exclusion, Predictive Symmetry.** Defines **SADP** and the **Predictive X-Y Typology** (Codes 1-9).                   |
|  **15.0**  | **Asked/stated vs Measured/observed (Data Source 3)**     | Codes the **raw data collection method** as **Asked/stated (1)** or **Measured/observed (2)** (Table 7).                                                                                              | **Exclusion Rule:** Modelled data must be Code 3 (**Statistically derived**).                                                                       |
|  **16.0**  | **Instructions for Producing Tables...**                  | Defines the **structure and content of all 8 output tables**.                                                                                                                                         | Includes the **Validation Rule** (Mandatory Pipe Check) and **Categorical Label Exclusion Constraint**.                                             |
|  **17.0**  | **Visual Decision Trees**                                 | Provides step-by-step **decision trees** for several key processes.                                                                                                                                   |                                                                                                                                                     |
|  **18.0**  | **Prompts for Producing and Validating AI Table Outputs** | Provides step-by-step prompts that the human user can utilize to efficiently progress through the process of providing necessary inputs and producing and validating AI table and flow chart outputs. |                                                                                                                                                     |

# **2.0 Instructions for Identifying Relevant Indicators**

I am asking AI to identify relevant indicators within research articles
that I will upload. We will define an indicator as **the use of a
variable for a management purpose.** The scope we are using to define
relevant management purposes is broad, including all of the management
purpose themes listed in the section [11.0 Management Purpose
Themes](#110-management-purpose-themes). This means that most variables
presented in a research article are likely to merit inclusion as
indicators based solely on that criterion. However, to be included they
must also meet an additional criterion: the indicator must be
**separately detailed,** meaning that the authors have provided **at
least one** of the following three basic indicator components. **All
variables explicitly documented are assumed to support the overarching
management purpose of the study**:

| Field Number | Component Field                                                     | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|:--------------------------:|:---------------------|:---------------------|
|    **1**     | **Name of indicator**                                               | This is one of three basic indicator components. If an indicator is explicitly named, e.g., identified as an indicator, this is grounds for inclusion of the indicator even if the definition and even if the specific variable assessment details are not provided.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|    **2**     | **Definition of indicator**                                         | This is one of three basic indicator components. If an indicator is defined, e.g., a description is provided about what a variable represents, this is grounds for inclusion of the indicator even if the indicator is not named and even if the specific variable assessment details are not provided).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|    **3**     | **Details of how the variable is assessed to inform the indicator** | This is one of three basic indicator components, and refers to the specific measurement protocol (e.g., scale, question, unit, formula, method). If the details of how a variable is assessed, i.e., scored for the purpose of evaluation, are described by authors, this can be grounds for inclusion if either: a) the indicator is scored via simple measurement, e.g., response to a survey question or weight of fish landings; b) the indicator is an outcome variable of a described equation; or c) the indicator is an element of equation for which a stand-alone score has been reported, as described in section [2.1.1 Scoring counts as a special type of variable assessment details](#211-scoring-counts-as-a-special-type-of-variable-assessment-details). **The presence of this information is NOT mandatory for inclusion if Name (1) or Definition (2) is present,** but many attributes of an indicator lacking variable assessment details will necessary require reporting those attributes as not reported ("n/r"). |

If all three of these basic indicator components are present, then the
AI will be able to fill in more of the attributes of the indicator in
subsequent instructions. If fewer indicator components are present, the
indicator can still be included in the list but subsequent attributes
may need to be listed as not reported "n/r."

## **2.1 Rules for special cases**

### **2.1.1 Scoring counts as a special type of variable assessment details**:

A variable for which a value (score) is reported counts as "Details of
how the variable is assessed" (Rule 3) for the purpose of ensuring
inclusion.

### **2.1.2 Parameter Inclusion Criterion**:

AI should not include **parameters** in the list of indicators **unless
the parameter is actively estimated, calibrated, or set using real-world
data specifically for the study's contextual or baseline assessment**.
This includes parameters estimated by minimizing log likelihoods,
setting to observed baseline averages, derived from secondary sources
where the specific value is selected, spatially or temporally
calibrated, or adjusted to fit the study's unique geographical,
environmental, or baseline conditions, or otherwise adjusted to anchor
the model to the local case study. Parameters treated as global, fixed
constants with no contextual specificity must be removed.

### **2.1.3 Hierarchical Constitutive Exception**:

Notwithstanding the **separately detailed criterion** described in [2.0
Instructions for Identifying Relevant
Indicators](#20-instructions-for-identifying-relevant-indicators), the
AI must include any intermediate aggregate variable or component (X) if
its inclusion is necessary to establish a complete, single-step
constitutive linkage chain (A  X  C) defined by the study's
quantitative model. This exception allows the inclusion of variables
that are inferred (i.e., not explicitly named, defined, or scored by the
authors) but are mathematically required as aggregation nodes to uphold
the integrity of the Standard Aggregate Decomposition Protocol (SADP)
described in section [14.2.1 Preparatory Mandates (Defining the Data
Set)](#1421-preparatory-mandates-defining-the-data-set) and the
Immediate Constitutive Link Rule described in section [14.2.2 Immediate
Constitutive Link Rule (Defining the Structural
Requirements)](#1422-immediate-constitutive-link-rule-defining-the-structural-requirements).

### **2.1.4 Narrative Causal Statement Inclusion Mandate**:

Notwithstanding the separately detailed criterion described in section
[2.0 Instructions for Identifying Relevant
Indicators](#20-instructions-for-identifying-relevant-indicators), the
AI must include any variable (X or Y) that is a component of a
**Narrative Causal Statement (NCS)**, as defined in section [14.3 X-Y
Relationship Types](#143-x-y-relationship-types). This mandate applies
when a directional relationship ($\text{X} \to \text{Y}$) asserted by
the research authors or study participants, linking a Narrative Causal
Element ($\text{X}$) to a Narrative Causal Outcome ($\text{Y}$) based on
findings derived directly from unstructured, primary qualitative data
(Narrative Variable Type, Code 4). This explicitly excludes assertions
or interpretations solely based on the synthesis of quantitative data
(e.g., economic models, descriptive statistics, or time-series analysis)
where no primary interview or observation data is presented. This
exception ensures the inclusion of indicators necessary to establish
systemic, non-quantitative causal linkages and must be coded as the
appropriate Inferred type for its **Inclusion Justification**.

### **2.1.5 Dual Variable Assessment Detail (VAD) Distinction Mandate**:

Notwithstanding the conceptual consolidation of attributes, the AI must
include the same concept as two separate, unique indicators if it is
documented with two fundamentally distinct Variable Assessment Details
(VADs) that lead to a difference in its fundamental variable type (Codes
1-4). This rule is non-negotiable when a concept is assessed:

-   **Quantitatively (VAD 1)**: Measured via a specific numerical
    protocol (Continuous/count (1), Ordinal (2), or Nominal (3) scale)
    and used as a constitutive input or quantitative predictor.
-   **Qualitatively/Narratively (VAD 2)**: Assessed via unstructured,
    long-form data (Narrative (4)), such as interview themes, case study
    context, or qualitative causality claims (NCS).

When this mandate applies, the two indicators **must be listed with
distinguishing names** (e.g., "Education Level - Ordinal Score" and
"Education Level - Narrative Element") and coded precisely to reflect
their respective Variable Type Upon Scoring (e.g., Code 2 vs. Code 4).

### **2.1.6 Narrative Synthesis Exclusion Constraint**:

Notwithstanding the Narrative Causal Statement Inclusion Mandate (Rule
2.1.4), the AI **must exclude** any variable whose asserted causal
relationship (X $\to$ Y) is based solely on the authors' interpretation,
synthesis, or qualitative discussion of quantitative results (e.g.,
trend data, statistical models, descriptive figures/tables) without
being explicitly grounded in primary qualitative data (interviews, field
notes, transcribed observation).

\### **2.1.7 Narrative Source Purity Constraint (for VTS Code 4)**: Any
indicator whose **Variable Type Upon Scoring** (Table 1) is **4
(Narrative)** must be the product of the current study's **direct
synthesis, content analysis, or thematic development** applied to **raw
qualitative/narrative data** (e.g., transcripts, field notes, narrative
reports).

<ul>

<li>If the current study accessed and analyzed **raw data it collected**
(Primary source), this mandate is met, and **Data Source 2 is Code
1**.</li>

<li>If the current study accessed and analyzed **raw data collected by a
third party** (Secondary source), this mandate is still met, but **Data
Source 2 is Code 2**.</li>

</ul>

**If the study only cites or analyzes a pre-existing summary, theme, or
finding synthesized by a third party, the variable cannot be Code 4**
and must be recoded as a Code 3 (Nominal), Code 2 (Ordinal), or Code 1
(e.g., frequency count of qualitative themes) variable based on how the
external claim is represented and treated in the current study's
analysis.

# **3.0 Variable Type Typology**

We are interested to record indicators that are directly assessed using
real-world measurements, as well as indicators that are calculated,
modeled, or categorized based on associated sub-variables. We refer to
indicators that are calculated using basic arithmetic as "calculated
outcomes," we refer to indicators resulting from more complex,
statistical modeling as "model outputs," and we refer to categorical
indicators that are conceptually based on a set of sub-variables as
"categorical outcomes." It is important to note that the "model output"
outcome status is inherited by any downstream calculated indicator
(Descriptive statistics, Composite index, Latent construct, or Other
derived outcome) that uses a Model Output as one of its direct or
indirect sub-variables. This ensures that any value tracing back to the
core simulation (and thus, subject to model complexity/uncertainty) is
categorized as a Model Output. For example, if Total Profit is the sum
of Patch Profits (which are Model Outputs), Total Profit is also coded
as a Model Output

AI **must use the lists** of basic variable types in section [3.1 Basic
Variable Types (Direct Measurement
Attributes)(#31-basic-variable-types-direct-measurement-attributes) and
outcome types in section [3.2 Outcome Variable
Types](#32-outcome-variable-types) to characterize each indicator
included in the list.

## **3.1 Basic Variable Types (Direct Measurement Attributes)**

| Code  | Term                       | Classification                  | Definition / Usage Note                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:-----------------:|:-----------------|:-----------------|:-----------------|
| **1** | **Continuous/count**       | Basic Variable Type             | Directly measured variable type where data points are meaningful numerical values. Continuous variables can take any value within a range (e.g., biomass, price), while Count variables are integers representing frequency (e.g., number of fishing trips). Also used to characterize the outcome of most derived variables (e.g., Indices (Outcome type Code 6), Latent Constructs (Outcome Type Code 7), Other Derived Outcomes (Outcome Type Code 8), or Model Outputs (Outcome Type Code 10)).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **2** | **Ordinal**                | Basic Variable Type             | Variable type where data points represent **categories with a meaningful rank or order** (e.g., Likert scale responses: High, Medium, Low; agreement ratings 1-5). The intervals between categories are often unequal or undefined. Also used to characterize the ordered outcome of derived variables (e.g., an Ordinal Index Score (Outcome Type Code 6); an Ordinal Latent Class (Outcome Type Code 7); a median descriptive statistic (Outcome Type Code 5)).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **3** | **Nominal**                | Basic Variable Type             | Variable type where data points represent **categories without any intrinsic order or rank** (e.g., Gender, Gear Type: Trawl vs. Seine, Management System: Open Access vs. Concession). Used as the input/state for categorical structure variables and to characterize the unordered categorical outcome of derived variables (e.g., a categorical outcome variable (Outcome Type Code 11); a Nominal Latent Class (Outcome Type Code 7); a mode descriptive statistic (Outcome Type Code 5)).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **4** | **Narrative**              | Basic Variable Type             | Variable type consisting of unstructured, long-form textual results. In the context of Narrative Causal Statements (NCS), Code 4 must be reserved exclusively for concepts/variables directly substantiated by findings derived from primary qualitative data collection, e.g., **unstructured, long-form textual results** arising from engagement with human subjects such as open-ended interview transcripts, field notes, observation logs. This variable type frequently serves as a **pre-scoring variable type** characterizing the raw data that is later transformed into a continuous/count, ordinal, or nominal form the purpose of scoring the indicator (i.e., for the **variable type upon scoring**). This variable type may also be relevant to variable type upon scoring in the context of a **Narrative causal statement** as defined in section [14.3 X-Y Relationship Types](#142-x-y-relationship-types), in which **narrative causal elements** are treated as relating variables and **narrative causal outcomes** are treated as target variables. In such cases, both **narrative causal elements (X)** and **narrative causal outcomes (Y)** would be coded as a narrative variable type (Code 4) in the variable type upon scoring. In the context of Narrative Causal Statements (NCS), Code 4 must be reserved exclusively for concepts/variables directly substantiated by findings derived from this form of primary qualitative data collection. |
| **5** | **Descriptive statistics** | Outcome Type (Code for Table 1) | A summary attribute of measured raw data (mean, median, sum, min/max). **Special Use Constraint**: This code is applied in the **Outcome Type** column **only** to indicate that a simple summary statistic of the basic variable type (codes 1-4) identified in **variable type upon scoring** is reported. [POPULATION MANDATE]: This code is applied in the Outcome Type column only to indicate that a simple summary statistic of a single variable is reported across a population or sample (e.g., Mean Catch Rate). [EXCLUSION]: It must not be used if the indicator represents a multi-faceted conceptual representation (Outcome Type Code 6), a latent construct (Outcome Type Code 7), a functional mathematical transformation (Outcome Type Code 8), a model output (Outcome Type Code 10), or a narrative causal outcome (Code 12). [SPECIAL USE AS BASELINE INPUT]: This code may also appear in the **Variable Type Upon Scoring** column if a summary statistic is used as a baseline or model input. **(Not to be treated as a calculated outcome for Conceptual Relationship Code 6.)**                                                                                                                                                                                                                                                                                                                                                                       |

## **3.2 Outcome Variable Types**

|  Code  | Term                         | Classification                  | Full Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|:-----------------:|:-----------------|:-----------------|:-----------------|
| **6**  | **Composite index**          | Outcome Type (Code for Table 1) | This is an outcome type that is mostly likely to be a continuous/count variable type, but can occasionally be an ordinal or nominal variable type. A composite index is calculated from a set of sub-variables, and conceptually the sub-variables are constitutive of the composite index, i.e., the composite index is conceptualized as a multi-faceted composite made up of the sub-variables as its component parts. [PURPOSE ALIGNMENT]: This code MUST be used if the aggregation's goal is to conceptually represent or summarize the aggregate state of a complex, multi-faceted concept. This holds even if the final output is binned into ordinal categories (e.g., "Low," "Medium," "High"), as these categories represent a summary of the underlying parts rather than an independent identity. [STATISTICAL MANDATE]: If this index is produced using a complex statistical method (e.g., Multidimensional Scaling [MDS], Factor Analysis, or Principal Component Analysis), it MUST be dual-coded as 6, 10. [OPERATIONAL TEST]: If a sub-variable (X) were removed, the Composite Index (Y) would conceptually become incomplete or redefined, but removing (X) does not imply (X) would cease to exist. [EXCLUSION]: Do not use this code if the primary purpose of the aggregation is to identify an Identity Type (e.g., a "regime" or "typology") where the result describes a kind of system based on a mix of attributes rather than an aggregate representation of its parts (see Code 11). [INCLUSION MANDATE]: This code MUST be applied if the study authors frame the variable as a summary representation of its constitutive inputs.                                                                                                             |
| **7**  | **Latent construct**         | Outcome Type (Code for Table 1) | This is an outcome type that is most likely to be a continuous/count variable type, but can occasionally be an ordinal or nominal variable type. A latent construct is calculated from a set of sub-variables, and conceptually the sub-variables are manifestations of the latent construct. [CAUSALITY MANDATE]: This code is distinguished from Code 6 by the Direction of Causality: sub-variables are seen as manifestations (reflective) of the construct rather than building blocks (constitutive). [STATISTICAL MANDATE]: If this construct is produced using a complex statistical method (e.g., Structural Equation Modeling, Factor Analysis, or Latent Class Analysis), it MUST be dual-coded as 7, 10. [OPERATIONAL TEST]: In the underlying causal model, the indicator itself (X) is hypothesized to be an effect of the unobservable construct (Y), meaning the construct drives the value of the observable indicator (Y → X). If one sub-variable is removed, the latent construct remains conceptually intact but is measured with less precision.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **8**  | **Other derived outcome**    | Outcome Type (Code for Table 1) | This is an outcome type that is most likely to be a continuous/count variable type, but can occasionally be an ordinal or nominal variable type. [FUNCTIONAL MATH MANDATE]: This code is reserved for outcomes produced through a mathematical transformation or structural ratio of two or more variables (e.g., Catch per Unit Effort [CPUE], density, percentage change, or standardized Z-scores). [STRUCTURAL TOTAL MANDATE]: This code includes "Cumulative Totals" or "Structural Sums" where different but physically related units are added together to create a single total (e.g., Total Assets = Gear + Boat + Engine; Total Catch = Species A + Species B). These represent a structural accumulation rather than the creation of a multi-faceted conceptual representation. [CONCEPTUAL DISTINCTION]: Unlike composite indices (Code 6), these variables provide functional or structural utility without creating a new, multi-faceted conceptual representation. The relationship between the sub-variables and the outcome is purely arithmetic or additive. [EXCLUSION]: Do not use this code if the calculation is framed as a summary of a multi-faceted concept (e.g., an "Index of Well-being" or "Vulnerability Rank"); such cases must be coded as Code 6. [INCLUSION RULE]: This code should be applied when the study authors make no explicit or implicit conceptual claim regarding a "composite" state, but are instead performing standard data normalization, structural sums, or functional calculations.                                                                                                                                                                                                                                     |
| **9**  | **Unknown**                  | Outcome Type (Code for Table 1) | This code should be applied if there is an outcome type but it is unknown.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **10** | **Model output**             | Outcome Type (Code for Table 1) | This code identifies the process of origin (statistical simulation/estimation) and must be applied alongside the outcome type that describes the variable's structure. Presence of this code indicates a value was produced through a complex statistical model, rather than a simple arithmetic calculation. This process status is inherited by any downstream indicator (Descriptive statistics (code 5), Composite index (code 6), Latent construct (code 7), Other derived outcome (code 8), or Categorical outcome (code 11)) that uses a Model Output as one of its direct or indirect sub-variables. This ensures that any value tracing back to the core simulation (and thus, subject to model complexity/uncertainty) is categorized as a Model Output. For example, if Total Profit is the sum of Patch Profits (which are Model Outputs), Total Profit is also coded as a Model Output. The "Model Output" code can be applied alongside any of the outcome types to indicate that the other outcome type was produced through complex statistical processes. For example, if a composite index was calculated using multi-dimensional scaling, such as in the case of the RAPfish framework, it would be identified as a composite index and also as a model output, with the code "6, 10." The Model output code #10 can co-occur with calculated outcomes (5, 6, 7, or 8) and can also co-occur with the Categorical outcome code #11 in the event that the classification process itself is modeled statistically (e.g., cluster analysis or factor analysis).                                                                                                                                                                                                |
| **11** | **Categorical Outcome**      | Outcome Type (Code for Table 1) | This is an outcome type of the basic variable type Nominal or Ordinal. This outcome reflects the classification or grouping of indicators to define a high-level category, type, or regime (e.g., policy scenario, governance type, or country grouping). [PURPOSE MANDATE]: This code is strictly reserved for indicators whose purpose is to assign identity or classify a system into a typology (e.g., "What kind of fishery is this?"). It defines a "kind" or "regime" based on a mix of attributes rather than a summary representation of a multi-faceted concept. [CONSTITUTIVE MANDATE]: To merit this code, the categories MUST be conceptually and/or arithmetically defined by drawing on the attributes of TWO or more distinct variables. [EXCLUSION]: Explicitly exclude outcome variables whose primary purpose is to represent a multi-faceted conceptual summary of constitutive parts (Code 6: e.g., Vulnerability Rank) or an unobservable latent state manifested through sub-variables (Code 7: e.g., Social Capital Index). [APPLICATION MANDATE]: This code MUST be applied to high-level classifications (e.g., Country Grouping, Fleet Segment) used in comparative analysis where the classification is defined to represent an aggregation of complex, non-enumerated characteristics, regardless of whether the study explicitly lists every constitutive sub-variable. [OPERATIONAL TEST]: If the categories represent different "states of being" or "identities" (e.g., Management Regime: Co-managed vs. Private) rather than an a "latent construct" or the "aggregate state" of a complex concept, use Code 11. [NOTE]: Can co-occur with Code #10 (Model Output) if the classification is modeled statistically (e.g., Cluster Analysis). |
| **12** | **Narrative causal outcome** | Outcome Type (Code for Table 1) | This is an outcome type of the basic variable type Narrative. This code identifies a qualitative response variable within the context of a Narrative Causal Statement (NCS), as described in section [14.3 X-Y Relationship Types](#142-x-y-relationship-types), in which **narrative causal elements (X)** are treated as relating variables and **narrative causal outcomes (Y)** are treated as target variables. [ROLE MANDATE]: Code 12 is reserved for the effect (Y) reported in a narrative causal statement found in the source text. It represents a non-quantified, conceptual outcome that is asserted to be influenced by a narrative causal element (X). The narrative causal outcome (Y) often corresponds to a high-level theme that lacks explicit arithmetical calculation. [CODING PROTOCOL]: \*\*Narrative causal outcomes (Y) must be coded as follows across the three main variable type columns: a. variable type upon scoring (Code 4); b. outcome type (Code 12); c. Variable type of outcome (Code 4). [PRE-SCORING NOTE]: In such cases, pre-scoring variable type should default to "n/r" unless there is explicit evidence that a distinct basic variable type preceded narrative.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

### **3.2.1 Derivation Constraints: Distinguishing Scoring Transformations from Multi-Variable Outcomes**

Notwithstanding the mandates described in the definitions of **Codes 6,
7, 8, and 11**, the AI must apply the following constraints when
determining the Outcome Type of binned or categorized variables. These
rules ensure that transformations applied to a **single variable**
during the scoring process are not miscoded as multi-faceted outcomes.

#### **3.2.1.1 Exclusion of Univariate Re-Binned Variables**

The AI must not apply complex Outcome Type codes (6, 7, 8, or 11) if the
final categories (bins) are formed solely by mathematically transforming
the range of values of a **single** directly assessed variable. Such
univariate transformation is a matter of indicator scoring and must be
classified as follows:

1.  **Descriptive Statistic (Code 5)**: If the re-binned categories are
    used to report a population summary (e.g., "40% of fishers fell into
    the High-Income bin"), the **Outcome Type** is Code 5.
2.  **Scoring Transformation (n/r)**: If the re-binned labels (e.g.,
    "Low," "Medium," "High") represent the final scored state for
    individual units, the **Outcome Type** column must be "n/r." The
    transformation is captured instead by the **Pre-scoring Variable
    Type** (e.g., Continuous) and the **Variable Type Upon Scoring**
    (e.g., Ordinal).
3.  **Identity Exception**: Code 11 (Categorical Outcome) is strictly
    reserved for instances where the identity or "kind" is defined by
    drawing on the attributes of **two or more** distinct variables.

#### **3.2.1.2 The Analytical Purpose Test (Identity vs. Status)**

When an outcome variable aggregates **two or more** distinct
sub-variables into discrete groups (Nominal or Ordinal), the AI must
determine the indicator's primary analytical purpose before assigning an
Outcome Type code:

-   **The Status Test (Code 6)**:
    -   **Question**: Is the goal to measure conceptual performance,
        risk, health, or success along a single dimension? (e.g., "How
        vulnerable is this site?")
    -   **Diagnostic**: If the categories represent levels of "more" or
        "less" of a multifaceted concept, the variable is a **Composite
        Index (Code 6)**.
-   **The Identity Test (Code 11)**:
    -   **Question**: Is the goal to define a state of being, a
        typology, a regime, or a policy scenario based on a specific
        configuration of attributes? (e.g., "What type of fleet is
        this?")
    -   **Diagnostic**: If the categories represent different "kinds" or
        "identities" rather than "levels of success," the variable is a
        **Categorical Outcome (Code 11)**.
-   **[MANDATE]**: In cases of ambiguity, the AI must prioritize the
    **Status Test**. If the categories represent an ordered ranking of a
    single multifaceted concept, **Code 6 (Composite Index)** takes
    precedence.

## **3.3 Variable Types at Different Points in Time**

For each indicator, AI **must pay attention to the variable type of the
indicator at three distinct points in time.** This will involve four
columns, as follows:

**Variable Type Upon Scoring**: This refers to the variable type at the
moment an indicator's value is assessed. Here are **three rules that AI
must follow** when filling in this column:

1.  **Primary Rule (Direct Measures)**: This column is primarily
    populated with the basic variable type (Continuous/count, Ordinal,
    Nominal, or Narrative) when the variable is a direct measurement
    (e.g., from a survey or field collection).
2.  **Secondary Rule (Calculated/Modeled)**: If the indicator is an
    Outcome variable (Calculated outcome, Model output, or Categorical
    outcome) **and its Outcome Type is Code 6, 7, 8, 10, or 11,** its
    entry must state "see sub-variables."
3.  **Note on Input Parameters in the context of Modeling**: This column
    is also used for the variable type of baseline data or model inputs
    at the moment they are assessed for use in a model. The point of
    assessment, or **scoring**, refers to the stage where a variable
    reaches the definitive form used as a direct numerical input for
    computation in the current study. For example, if a complex
    pre-calculated estimate is used as an input score, its outcome type
    code (#6, #7, #8, #10, or #11) should be listed here instead of a
    basic variable type; if a summary statistic is used as baseline data
    or model input, the descriptive statistics code (#5) should be
    listed here instead of a basic variable type code). For any code
    listed here, it will be assumed to be a continuous/count variable
    type unless a "n" is amended to the code indicating that it is a
    nominal variable (e.g., "5n" indicating a nominal descriptive
    statistic such as a "mode"; "11n" indicating a nominal categorical
    outcome variable), or an "o" is amended to the code number
    indicating that it is an ordinal variable (e.g., "5o" indicating an
    ordinal descriptive statistic, such as the median score across an
    ordinal scale). Notwithstanding the above, if the input parameter is
    a basic variable type (Codes 1-4) that is used exclusively to define
    the organizational, contextual, or categorical structure of the
    current study or model (e.g., location, time period, experimental
    treatment/scenario), then the basic variable type (e.g., Code 3 for
    Nominal) must be retained and must not be replaced by an Outcome
    Type code. If a complexity code (Code 5, 6, 7, 8, 10, or 11) is used
    here to define an input score, the **Non-Redundancy Constraint** for
    the **Outcome type** column (Rule 4) must be applied.

**Pre-scoring Variable Type**: This column records the variable type of
the original raw data source **only if** a transformation occurred that
resulted in a **distinct** basic variable type for the purpose of the
indicator's scoring. Here are **two rules that AI must follow** when
filling in this column:

1.  **Primary Rule (Transformation)**: If a raw variable type was
    transformed into a **distinct basic variable type** for the purpose
    of scoring an indicator (e.g., narrative data was transformed into
    nominal categorical data, or continuous/count data were transformed
    into ordinal categories), use the basic variable types
    (Continuous/count, Ordinal, Nominal, or Narrative) to identify the
    variable type that best characterizes the raw data type (if
    different from the variable type upon scoring).
2.  **Exclusion Rule (No Distinction)**: If the transformation resulted
    in a variable type identical to the original raw data type (e.g.,
    Ordinal -\> Ordinal, Nominal -\> Nominal), or if the original raw
    data type is unknown/not reported, the entry must state "n/r". This
    ensures the column only highlights a change in the type of variable
    used.
3.  **Outcome Rule (Derived Indicators)**: If the indicator is an
    Outcome variable (Code 6, 7, 8, 10, 11, or 12), the entry must state
    "see sub-variables." This directs the reader to examine the inputs
    (sub-variables) of the derived metric rather than the metric itself.

**Outcome Type**: This column identifies the method by which a final
value or categorization was produced. Here are **four rules that AI must
follow** when filling in this column:

1.  **Complex Outcome Rule**: If the indicator is a Model output,
    Categorical outcome, or Calculated Outcome (e.g., Composite index,
    Latent construct, or other Derived Outcome), record the
    corresponding numeric code (6, 7, 8, 10, or 11). **(Note: This rule
    excludes Descriptive Statistics (Code 5)).**
2.  **Descriptive Statistics Rule**: If the indicator is a direct
    measurement (whose Variable type upon scoring is a basic type) but
    results in a simple data summary (mean, sum, median) being reported,
    record "Descriptive Statistics" here (code #5).
3.  **Default**: If neither a complex outcome variable nor a descriptive
    statistic is applicable, write "n/r" (without any associated
    numerical code or modifier).
4.  **Non-Redundancy Constraint (Input Scores)**: If the Variable type
    upon scoring column contains a complexity code (Code 5, 6, 7, 8, 10,
    or 11) to define a pre-calculated aggregate or model input score (as
    defined in the Note on Input Parameters), the entry in the Outcome
    type column must be "n/r." This constraint prevents the duplicate
    recording of a complex variable type that is used as an input score
    rather than being the reported outcome of the current analysis.

**Variable Type of Outcome**: This column identifies the basic variable
type of the final result of the calculation or modeling process. Here
are **two rules that AI must follow** when filling in this column:

1.  **Required Entry**: If the Outcome type columns contains the entry
    Descriptive Statistics (Code #5), Composite index (Code #6), Latent
    construct (Code #7), Other Derived Outcome (Code #8), Model output
    (Code #10), Categorical outcome (Code #11), or a combination of Code
    #10 with one of the other codes listed here, identify the basic
    variable type (Continuous/count, Ordinal, Nominal, or Narrative) of
    the final reported value. Note: When listing the basic variable type
    code (#1, #2, #3, or #4) in this column, no suffixes (e.g., "n" or
    "o") should be applied.
2.  **Default**: If there is no entry in the Outcome type column, write
    "n/r" (without any associated numerical code or modifier).

# **4.0 Conceptual Relationship Coding**

## **4.1 Constraint on Conceptual Coding (Predictive Independence)**:

The coding of conceptual relationship type (Codes 1 through 7, as
defined in the sub-section [4.2 Conceptual Relationship
Typology](#4.2-conceptual-relationship-typology), **must be determined
solely by the indicator's internal characteristics (proxy status) and
its role in constitutive relationships (Associated
Outcome/Sub-variable). These codes must be treated as independent of,
and should not be influenced by, whether the indicator is used as a
Relating variable (X) or a Target variable (Y) in the study's X-Y
predictive analyses.**

### **4.1.1 Conceptual Relationship Priority Mandate (Code 6/8 Distinction)**:

When classifying an aggregate variable whose calculation involves a
formula, statistical technique (e.g., MDS, Factor Analysis), or other
complex derivation, the determination between Composite Index (Code 6)
and Other Derived Outcome (Code 8) MUST prioritize the study authors'
explicit or implicit conceptual framing of the output over the
mathematical complexity.

If the study explicitly or implicitly frames the aggregate index as
representing a conceptual whole that is composed of or summarized by its
input sub-variables (i.e., making a claim of conceptual representation),
the index MUST be coded as a Composite Index (Code 6). This
classification holds even if the calculation uses complex scaling,
weighting, or statistical transformation (e.g., RAPFISH/MDS) that
mathematically breaks a simple additive link.

Code Other Derived Outcome (Code 8) is reserved only for aggregated
outputs where the study makes no conceptual claim of composition, or
where the output is strictly mathematical (e.g., complex ratios, simple
structural transformations, or residual components lacking conceptual
definition).

## **4.2 Conceptual Relationship Typology**

The following typology should be used to characterize the presence or
absence of a within-indicator conceptual relationship (i.e., conceptual
proxy) and/or the role of an indicator in a constitutive conceptual
relationship with a separate indicator (i.e., the role of an indicator
as a sub-variable or an outcome variable). The AI **must use the code
numbers rather than text to indicate relevant conceptual relationships**
in Table 4. The conceptual relationship codes are as follows:

| Code  | Term                                   | Role / Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Co-occurrence Rules                                                                    |
|:-----------------:|:-----------------|:-----------------|:-----------------|
| **1** | **No proxy single variable**           | Directly measured, variable concept equals indicator topic, and NOT a constitutive sub-variable. **Priority Rule (Descriptive Stats):** This code **MUST** be used, and Code 7 **MUST NOT** be used, if the indicator meets this definition and the only reason it would not be a single variable is the presence of an **Outcome Type Code 5 (Descriptive statistics).**                                                                                                                                   | **Cannot co-occur** with any other code.                                               |
| **2** | **Conceptual proxy single variable**   | Directly measured, and the variable concept is located in a distinct sub-category from the indicator topic (Proxy present). Priority Rule (Descriptive Stats): This code MUST be used, and Code 7 MUST NOT be used, if the indicator meets this definition, regardless of the presence of an Outcome Type Code 5 (Descriptive statistics).                                                                                                                                                                  | **Can co-occur** with codes #3, #4, #5, #6. **Cannot co-occur** with code #7.          |
| **3** | **Sub-variable of a latent construct** | Constitutive sub-variable used to calculate a latent construct. **Mandate**: This code applies if the immediate Associated Outcome Variable's Outcome Type is Latent construct (Code 7), whether modeled (Code 7, 10) or non-modeled (Code 7). **Dual Role Clarification**: This indicator may itself be a calculated outcome (Code 6) from a previous step, necessitating the co-occurrence code $\mathbf{6; 3}$.                                                                                          | **Can co-occur** with code #2 or #6. **Cannot co-occur** with codes #1, #4, #5, or #7. |
| **4** | **Sub-variable of a composite index**  | Constitutive sub-variable used to calculate a composite index. **Mandate**: This code applies if the immediate Associated Outcome Variable's Outcome Type is Composite Index (Code 6), whether modeled (Code 6, 10) or non-modeled (Code 6). **Dual Role Clarification**: This indicator may itself be a calculated outcome (Code 6) from a previous step, necessitating the co-occurrence code $\mathbf{6; 4}$.                                                                                            | **Can co-occur** with code #2 or #6. **Cannot co-occur** with codes #1, #3, #5, or #7. |
| **5** | **Sub-variable of a derived outcome**  | Constitutive sub-variable used to calculate a derived outcome other than a latent construct or a composite index. **Mandate**: This code applies if the immediate Associated Outcome Variable's Outcome Type is Other Derived Outcome (Code 8), whether modeled (Code 8, 10) or non-modeled (Code 8), or Categorical Outcome (Code 11). **Dual Role Clarification**: This indicator may itself be a calculated outcome (Code 6) from a previous step, necessitating the co-occurrence code $\mathbf{6; 5}$. | Can co-occur with code #2 or #6. Cannot co-occur with codes #1, #3, #4, or #7.         |
| **6** | **Outcome variable**                   | The indicator is a calculated outcome, model output, or categorical outcome connected to other sub-variables in this list (or clearly implied). Constraint: This code applies **ONLY** if the Outcome Type includes the Code 6, 7, 8, or 11. It **MUST NOT** be applied if the Outcome Type is Code 5 (Descriptive statistics).                                                                                                                                                                             | **Can co-occur** with code #2, #3, #4, or #5. **Cannot co-occur** with code #7.        |
| **7** | **Other**                              | Reserved for residual cases that are not constitutive (no Code 3, 4, 5, 6) and whose conceptual components (Primary Variable Concept or Indicator Topic) are so poorly detailed that they **cannot be matched to any other category (Code 1 or 2).**                                                                                                                                                                                                                                                        |                                                                                        |

## **4.3 Constitutive Code Synchronization Rule**

**Priority Rule for Co-occurring Outcome Types (Codes 6, 7, and 10)**:
When an Associated Outcome Variable (Y) is coded as a **Model Output
(10)** and also includes a Conceptual Type (Code 6 or 7), the input
Indicator's (X) constitutive code (**3 or 4**) must reflect the
Conceptual Type (6 or 7), rather than the Model Output's generic input
code (**5**). Codes 3 and 4 take precedence over Code 5. This maintains
the integrity of the conceptual typology (Latent Construct or Composite
Index) over the method of calculation (Modeled).

**Synchronization Reference Table**: If an indicator acts as a
sub-variable for another indicator, the assignment of the conceptual
relationship code (3, 4, or 5) must be explicitly synchronized with the
Outcome Type of its immediate Associated Outcome Variable(s) reported in
Table 1. This check ensures that the input (sub-variable) relationship
code perfectly matches the output (outcome variable) typology. The
synchronization Reference Table is as follows:

|       If Output Indicator (Y) is Code...        |  ...Then Input Indicator (X) Must Be Code...   | Full Definition of Rule                                                                                                                                                                                                                                                                                                                                                                                   |
|:------------------------:|:------------------------:|:--------------------|
|    **6** (**Composite Index**), or **6, 10**    | **4** (**Sub-variable of a composite index**)  | If the immediate Associated Outcome Variable (Y) is a Composite Index (**6** or **6, 10**) in Table 1, the sub-variable (X) is a constitutive building block of a multifaceted concept (**Parts → Whole**). In this case, the sub-variable (X) must be coded as **4** (Sub-variable of a composite index). (Priority over Code 5)                                                                         |
|   **7** (**Latent Construct**), or **7, 10**    | **3** (**Sub-variable of a latent construct**) | If the immediate Associated Outcome Variable (Y) is a Latent Construct (**7** or **7, 10**) in Table 1, the sub-variable (X) is an observable manifestation of the unobservable state (**Whole → Parts**). In this case, the sub-variable (X) must be coded as **3** (Sub-variable of a latent construct). (Priority over Code 5)                                                                         |
| **8** (**Other Derived Outcome**), or **8, 10** | **5** (**Sub-variable of a derived outcome**)  | If the immediate Associated Outcome Variable (Y) is an Other Derived Outcome (**8**) in Table 1, the sub-variable (X) is a component of a functional ratio, structural tally, or other strictly arithmetic calculation that does not imply the calculation of a multifaceted concept (Arithmetic Utility). In this case, the sub-variable (X) must be coded as **5** (Sub-variable of a derived outcome). |
|            **10** (**Model output**)            | **5** (**Sub-variable of a derived outcome**)  | If the immediate Associated Outcome Variable (Y) is coded as Model Output (**10**) alone (no 6 or 7), the input (X) is a generic modeled numerical parameter. In this case, the sub-variable (X) must be coded as **5** (Sub-variable of a derived outcome).                                                                                                                                              |
| **11** (**Categorical Outcome**), or **11, 10** | **5** (**Sub-variable of a derived outcome**)  | If the immediate Associated Outcome variable (Y) is a Categorical Outcome (**11** or **11, 10**) in Table 1, the sub-variable (X) is an **Identity Attribute** used to define a typology or kind. In this case, the sub-variable (X) must be coded as **5** (Sub-variable of a derived outcome). **[RATIONALE MANDATE]**: The rationale must specify that (X) defines a typological identity/regime.      |

# **5.0 Community Type**

The following typology should be used to characterize the **Community
Type** of the indicator:

|  Code   | Community Type                          | Definition                                                                                                                                                                                                    |
|:--------------------------:|:---------------------|:---------------------|
|  **1**  | **Fishery Participant Community Focus** | The **indicator topic** is relevant to a **fishing community-of-practice** (i.e., fishery actors or the fishery as a whole).                                                                                  |
|  **2**  | **Place-based Community Focus**         | The **indicator topic** is relevant to a **place-based fishing community** (i.e., including non-fishing community members and/or having to do with the community context of place-based fishing communities). |
|  **3**  | **Unclear**                             | The **indicator topic** is challenging to clearly locate as community type Code #1, Code #2, or Code #4 due to lack of specificity in the source text.                                                        |
|  **4**  | **Context Variable**                    | The **indicator topic** relates to the broader **Human Dimensions Context** or the **Environmental Context** in which a community exists.                                                                     |
| **n/r** | **Not reported**                        | No information is available about the community focus of the indicator.                                                                                                                                       |

## **5.1 Primary Category as Guide to Community Type Coding**

While an **indicator topic** coded to sub-categories within some of the
**primary categories** have potential to be coded as any of the
**community type** codes, there are also some primary categories that
are inherently conceptually related to a specific community type, e.g.,
the **Community Context** primary category is specifically defined as
relevant to descriptions of a place-based fishing community (Code #2).
The following groupings identify primary categories that are either
specifically tied to one of the community type codes, or for which
multiple community type codes may make sense for an indicator:

-   **Primary Categories with a Fishery Participant Community Focus
    (Code 1)**: Indicators for which the **Indicator Topic** is coded to
    conceptual sub-categories within the following primary categories
    **must receive Code #1**:

    -   **Fishery Governance System Characteristics**
    -   **Fishery Governance System Performance**
    -   **Fishery System Economic Performance**
    -   **Fishery System Environmental Performance**
    -   **Fishery System Social Performance**

-   **Community Context Indicators (Code 2)**: Indicators coded to
    conceptual sub-categories within the **Community Context** primary
    category **must receive Code #2**.

-   **Macro-Context Indicators (Code 4)**: Indicators coded to
    conceptual sub-categories within the **Environmental Context**
    primary category or the **Human Dimensions Context** primary
    category **must receive Code #4**.

-   **Primary Categories with multiple possible community types**:
    Indicators for which the Indicator Topic is coded to the following
    sub-categories may be coded as either Code #1, Code #2, depending on
    the focus of the indicator itself:

    -   **Fishery Participant Well-being Capabilities**
    -   **Fishery Participant Well-being Conditions**
    -   **Fishery Participant Well-being Connections**

-   **Mandatory Rule: Contextual Resolution for Well-being Indicators**:
    When assigning a Community Type Code (Code #1 or Code #2) to
    indicators categorized under the three Fishery Participant
    Well-being primary categories, the system **MUST NOT** apply a
    conceptual default based on the indicator's topic (e.g., assuming
    socioeconomic variables automatically require Code #2). Instead, the
    code assignment **MUST** be determined by the **explicit data
    collection target** (the sampling frame) identified in the data
    source description or indicator narrative:

    -   **Rule A (Code 1 Requirement)**: If the indicator data was
        collected exclusively from identified Fishery Participants
        (e.g., individual fishers, patrons) or their designated
        Households/Entities, the code must be Code #1 (Fishery
        Participant Community Focus). This acknowledges that the data
        defines the characteristics of the specialized community of
        practice.
    -   **Rule B (Code 2 Requirement)**: If the indicator data was
        collected from a sampling frame that includes the general
        residential population of the local area (i.e., fishers and
        non-fishers, typically from census data or a community-wide
        survey), the code must be Code #2 (Place-based Community Focus).
        This acknowledges the focus is on the general socioeconomic
        context of the location.

## 5.2 **Example of Determining Community Type Code**

-   **Per Capita Income**: An indicator of per capita income must be
    coded as Code 1 (fishery community-of-practice) if it is specified
    as per capita income of fishers, and it must be coded as Code 2
    (place-based fishing community) if it is specified as per capita
    income of all members of a community.

# **6.0 Unit of Observation**

The following typology should be used to select the code for the **Unit
of Observation** that best characterizes the **variable assessment
details** of an indicator:

|         Code          | Conceptual Scale     | Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|:--------------------------:|:---------------------|:---------------------|
|         **1**         | **Individual**       | The assessment/scoring of the **variable** occurs at the conceptual scale of an individual person (e.g., individual fisher; individual community member).                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|         **2**         | **Household**        | The assessment/scoring of the **variable** occurs at the conceptual scale of a household (e.g., fisher household; all households in a community).                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|         **3**         | **Sub-group**        | The assessment/scoring of the **variable** occurs at the conceptual scale of a sub-group (e.g., fishers grouped into kinship groups; members of a community organization).                                                                                                                                                                                                                                                                                                                                                                                                                     |
|         **4**         | **Community**        | The assessment/scoring of the **variable** occurs at the conceptual scale of a community (e.g., all fishers in the fishing community-of-practice; all community members in a place-based fishing community).                                                                                                                                                                                                                                                                                                                                                                                   |
|         **5**         | **Unclear**          | The conceptual scale of **variable** assessment/scoring for this indicator is challenging to clearly locate as Code 1, Code 2, Code 3, Code 4, or Code 6 due to lack of specificity in the source text (e.g., the variable is described but not in sufficient detail to clarify the scale).                                                                                                                                                                                                                                                                                                    |
|         **6**         | **Supra-community**  | The assessment/scoring of the **variable** occurs at a conceptual scale higher than that of a community (e.g., assessment of fishery governance concepts across multiple discretely defined fisheries, such as across multiple national jurisdictions; assessment of a human dimensions concepts at a macro scale beyond the scale of an individual fishery or fishing community, such as at a regional, national or international scale, warranting coding in the Human Dimensions Context primary category).                                                                                 |
|        **n/r**        | **Not reported**     | No information is available about the conceptual scale at which the **variable** was assessed/scored for this indicator (e.g., the indicator is included in the list because it was named and/or defined, but no information is presented in the source text about the **variable assessment details**).                                                                                                                                                                                                                                                                                       |
| **see sub-variables** | **Outcome variable** | The indicator is an outcome variable calculated or conceptually constituted by its sub-variables, and therefore information about unit of observation of variables requires examining the sub-variables (e.g., the indicator is a composite index, latent construct, or other derived outcome, and the unit of observation would only be relevant when examining the sub-variables used to calculate it; the indicator is a categorical outcome and the unit of observation depends on the sub-variables upon which the nominal categories of the categorical outcome are conceptually based). |
|        **n/a**        | **Not applicable**   | The **variable concept** is coded to the Environmental Context primary category and therefore the levels of human social organization are not applicable.                                                                                                                                                                                                                                                                                                                                                                                                                                      |

## **6.1 Special Rules for Unit of Observation**

### **6.1.1 Inclusion Constraints**

-   **6.1.1.1 Inclusion Constraint 1**: If the indicator's **Outcome
    type** is any form of calculated outcome (Composite index, Latent
    construct, Other derived outcome), a Model output, or a Categorical
    outcome, this column **must state "see sub-variables."**
-   **6.1.1.2 Inclusion Constraint 2**: If the indicator's Variable Type
    Upon Scoring is populated with an Outcome Type code (Code 5, 6, 7,
    8, 10, or 11) because it represents a pre-calculated aggregate used
    as a baseline or model input (and Rule 6.1.1.1 does not already
    apply), this column must state "see sub-variables." This rule
    prevents analyzing the Unit of Observation for a metric that was
    already aggregated in a previous study or context.
-   **6.1.1.3 Inclusion Constraint 3**: If the indicator's **primary
    variable concept** is coded to a sub-category within the
    Environmental Context primary category, the levels of human social
    organization are not applicable and this column **must state
    "n/a".**

### **6.1.2 Overarching Rule: Differentiating Sub-Group (3), Community (4), and Supra-community (6)**

When a variable is assessed at a higher scale than individual (Code #1)
or household (Code #2), e.g., if the variable is assessed at the level
of a sub-group (Code #3), the entire **fishery-community of practice**
or a full **place-based community** (Code #4) or at a level higher than
the community (Code #6), the determination of appropriate level depends
*exclusively* on how the source study defines and treats the aggregation
unit.

**A. Rule for Code 3 (Sub-group Level):** An indicator is coded as
**Sub-group (3)** if the indicator focuses on a sub-unit of a larger
fishery, i.e., the study's narrative explicitly or implicitly treats the
sub-unit as one component of the larger fishery, and that larger fishery
is treated as a **single, cohesive conceptual entity**.

-   **Case 3a (Place-Based):** If a group of small villages is
    characterized *by the study* as one cohesive place-based community,
    then an indicator focusing on only one of the villages is coded at
    the **Sub-group level (3)**.
-   **Case 3b (Community-of-Practice):** If a singular fishery is
    defined *by the study* as involving multiple distinct gear types,
    then an indicator focusing on only one of the distinct gear types is
    coded at the **Sub-group level (3)**.

**B. Rule for Code 4 (Community Level):** An indicator is coded as
**Community (4)** if the study's narrative explicitly or implicitly
treats the aggregation of sub-units as a **single, cohesive conceptual
entity**.

-   **Case 4a (Place-Based):** If a group of small villages is
    characterized *by the study* as one cohesive place-based community,
    then any indicator aggregating information from those villages is
    coded at the **Community level (4)**.
-   **Case 4b (Community-of-Practice):** If a singular fishery is
    defined *by the study* as involving multiple distinct gear types,
    then an indicator aggregating information across those gear types is
    coded at the **Community level (4)**.

**C. Rule for Code 6 (Supra-community Level): An indicator is coded as**
Supra-community (6)\*\* if the study's narrative explicitly or
implicitly treats the aggregation of units as a collection of
**multiple, distinct conceptual entities**.

-   **Case 6a (Multiple Communities):** If the study characterizes a
    group of villages as each constituting its own *distinct place-based
    fishing community*, then an indicator aggregating information from
    all villages must be coded as **Supra-community (6)**.
-   **Case 6b (Multiple Fisheries):** If the study defines each gear
    group as its own, *separate fishery*, then an indicator combining
    information from all these separate fisheries must be coded as
    **Supra-community (6)**.

**Principle of Scope:** Code 6 will typically be reserved for studies
with regional, national, or international focus, or for studies that
look across conceptual units (communities or fisheries) that are
explicitly managed or analyzed separately from one another.

### 6.1.3 **Rules for Data Collection Methods (Codes 1, 3, and 4)**

The selection among Individual (1), Sub-group (3), and Community (4) is
determined by the variable assessment method described in the source
text, specifically whether the assessment targets a single unit, a
designated component, or the entire collective unit.

-   **Rule 6.1.3.1 Individual Level (Code 1)**: If the **variable
    assessment details** involved direct, non-aggregated assessment of a
    single individual (e.g., measuring catch volume per fishing trip,
    surveying a single fisher), the indicator must be coded as Unit of
    Observation Code 1 (Individual level).
-   **Rule 6.1.3.2 Sub-group Level (Code 3)**: If the **variable
    assessment details** involved direct assessment applied collectively
    to a pre-defined subset or component of the community (e.g., a
    single survey conducted only with members of one gear group, a
    single estimate provided only for one specific village/location
    within the overall community), the indicator must be coded as Unit
    of Observation Code 3 (Sub-group level).
-   **Rule 6.1.3.3: Community Level (Code 4)**: If the **variable
    assessment details** involved a single, direct assessment applied to
    the entire collective unit (e.g., a complete census of the fishery,
    a single expert estimate of the total harvest for the whole
    community or fishery), the indicator must be coded as Unit of
    Observation Code 4 (Community level).

## 6.2 **Examples of Determining Unit of Observation**

| Primary Variable Concept | Variable Assessment Details                                                                                                                                                   | Unit of Observation Code | Unit of Observation Description |     |
|---------------|---------------|---------------|:-------------:|---------------|
| Harvest volume           | Volume of catch delivered by individual fishers                                                                                                                               | 1                        |        Individual level         |     |
| Harvest volume           | Expert estimate of total volume harvested by a single gear group, where multiple gear groups are defined as included within the overall aggregation unit for the fishery      | 3                        |         Sub-group level         |     |
| Harvest volume           | Expert estimate of the total volume harvested in the fishery overall                                                                                                          | 4                        |         Community level         |     |
| Harvest volume           | Total volume of catch of a specific target species that is received by processing plants, where the aggregation unit for the fishery is defined by that single target species | 4                        |         Community level         |     |

# **7.0 Unit of Analysis**

The following typology should be used to select the best code for the
**Unit of Analysis** of the **indicator topic**:

|  Code   | Conceptual Scale    | Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|:--------------------------:|:---------------------|:---------------------|
|  **1**  | **Individual**      | The presentation of the **indicator topic** occurs at the conceptual scale of an individual person (e.g., individual fisher; individual community member).                                                                                                                                                                                                                                                                                                                                                                         |
|  **2**  | **Household**       | The presentation of the **indicator topic** occurs at the conceptual scale of a household (e.g., fisher household; all households in a community).                                                                                                                                                                                                                                                                                                                                                                                 |
|  **3**  | **Sub-group**       | The presentation of the **indicator topic** occurs at the conceptual scale of a sub-group (e.g., fishers grouped into kinship groups; members of a community organization).                                                                                                                                                                                                                                                                                                                                                        |
|  **4**  | **Community**       | The presentation of the **indicator topic** occurs at the conceptual scale of a community (e.g., all fishers in the fishing community-of-practice; all community members in a place-based fishing community).                                                                                                                                                                                                                                                                                                                      |
|  **5**  | **Unclear**         | The conceptual scale of **indicator topic** presentation is challenging to clearly locate as Code 1, Code 2, Code 3, Code 4, or Code 6 due to lack of specificity in the source text (e.g., the indicator is named but no information is presented about its assessment/scoring or final presentation).                                                                                                                                                                                                                            |
|  **6**  | **Supra-community** | The presentation of the **indicator topic** occurs at a conceptual scale higher than that of a community (e.g., representing fishery governance concepts across multiple discretely defined fisheries, such as across multiple national jurisdictions; representing a human dimensions concept at a macro scale beyond the scale of an individual fishery or fishing community, such as at a regional, national or international scale, warranting coding in the Human Dimensions Context primary category).                       |
| **n/r** | **Not reported**    | No information is available about the conceptual scale at which the **indicator topic** was presented (e.g., the indicator is included in the list because it was named and/or defined, but no information is presented in the source text about the final presentation of the indicator). This may be the case if either 1. no variable assessment details were included, or 2. the variable assessment details were included but there was no final presentation of the indicator beyond initial scoring/assessment information. |
| **n/a** | **Not applicable**  | The **indicator topic** is coded to the Environmental Context primary category and therefore the levels of human social organization are not applicable.                                                                                                                                                                                                                                                                                                                                                                           |

## **7.1 Special Rules for Unit of Analysis**

### **7.1.1 Exclusion and Default Constraints**

-   **Rule 7.1.1.1 Exclusion Constraint (Environmental Context)**: If
    the **Indicator Topic** is coded to any sub-category within the
    Environmental Context primary category, the Unit of Analysis column
    must state "n/a." This constraint applies because environmental
    characteristics are not relevant to measuring or interpreting the
    scale of human social organization.
-   **Rule 7.1.1.2 Default Constraint (Fishery Governance)**: If the
    **Indicator Topic** is coded to a sub-category within the Fishery
    Governance System Characteristics or Fishery Governance System
    Performance primary categories, the indicator **defaults to the
    Community level (Code 4)**. This default applies **only if** the
    final presentation of the indicator (as determined by Rules 7.1.2
    and 7.1.3) does **not** clearly specify the scale of presentation as
    Individual (Code 1), Household (Code 2), Sub-group (Code 3), or
    Supra-community (Code 6). This is because fishery governance systems
    are inherently designed to manage the entire
    fishery-community-of-practice unless stated otherwise.
-   **Rule 7.1.1.3 Default Constraint (Human Dimensions Context)**: If
    the **Indicator Topic** is coded to any sub-category within the
    Human Dimensions Context primary category, the indicator **defaults
    to the Supra-community level (Code 6).** This default applies **only
    if** the source text **does not** clearly specify the scale of
    presentation as Individual (Code 1), Household (Code 2), Sub-group
    (Code 3), or Community (Code 4). This is because the Human
    Dimensions Context is inherently designed to emphasize macro-scale
    factors (regional, national, international) that typically transcend
    an individual fishery community-of-practice or an individual
    place-based fishing community scale.

### **7.1.2 Definitive Rule: Differentiating Scale of Presentation (Codes 1, 3, 4, and 6)**

When the presentation of an indicator is at a scale higher than
Household (Code #2), the determination of the appropriate level depends
exclusively on how the source study defines and treats the final
aggregation unit.

-   **Note on Aggregation**: This rule applies when the initial data
    collection (Unit of Observation) is at the individual level (Code
    #1) or household level (Code #2) but is then aggregated for final
    presentation.

**A. Rule for Code 3 (Sub-group Level):** An indicator is coded as
**Sub-group (3)** if the indicator focuses on a sub-unit of a larger
fishery, i.e., the study's narrative explicitly or implicitly treats the
sub-unit as one component of the larger fishery, and that larger fishery
is treated as a **single, cohesive conceptual entity**.

-   **Case 3a (Place-Based):** If a group of small villages is
    characterized *by the study* as one cohesive place-based community,
    then an indicator focusing on only one of the villages is coded at
    the **Sub-group level (3)**.
-   **Case 3b (Community-of-Practice):** If a singular fishery is
    defined *by the study* as involving multiple distinct gear types,
    then an indicator focusing on only one of the distinct gear types is
    coded at the **Sub-group level (3)**.

**B. Rule for Code 4 (Community Level):** An indicator is coded as
**Community (4)** if the study's narrative explicitly or implicitly
treats the aggregation of sub-units as a **single, cohesive conceptual
entity**.

-   **Case 4a (Place-Based):** If a group of small villages is
    characterized *by the study* as one cohesive place-based community,
    then any indicator aggregating information from those villages is
    coded at the **Community level (4)**.
-   **Case 4b (Community-of-Practice):** If a singular fishery is
    defined *by the study* as involving multiple distinct gear types,
    then an indicator aggregating information across those gear types is
    coded at the **Community level (4)**.

**C. Rule for Code 6 (Supra-community Level):** An indicator is coded as
**Supra-community (6)** if the study's narrative explicitly or
implicitly treats the aggregation of units as a collection of
**multiple, distinct conceptual entities**.

-   **Case 6a (Multiple Communities):** If the study characterizes a
    group of villages as each constituting its own *distinct place-based
    fishing community*, then an indicator aggregating information from
    all villages must be coded as **Supra-community (6)**.
-   **Case 6b (Multiple Fisheries):** If the study defines each gear
    group as its own, *separate fishery*, then an indicator combining
    information from all these separate fisheries must be coded as
    **Supra-community (6)**.

**Principle of Scope:** Code 6 will typically be reserved for studies
with regional, national, or international focus, or for studies that
look across conceptual units (communities or fisheries) that are
explicitly managed or analyzed separately from one another.

### 7.1.3 **Rule for Aggregation vs. Non-Aggregation (Codes 1, 3, and 4)**

The selection of the scale of presentation, either Individual (1),
Sub-group (3), or Community (4), is determined by the final form of the
indicator:

-   **Rule 7.1.3.1: Individual Level (Code 1)**: If the **Indicator
    Topic** is Harvest volume and the final presentation of the
    indicator lists the individual catch volume of individual fishers
    (i.e., data is presented per fisher, not aggregated across fishers),
    the indicator must be coded as Unit of Analysis Code 1 (Individual
    level).

-   **Rule 7.1.3.2: Sub-group Level (Code 3)**: If the **Indicator
    Topic** is Harvest volume and the final presentation of the
    indicator lists the total catch OR a summary statistic aggregated
    only across a defined sub-group of fishers (e.g., total harvest of
    only the longline fleet), the indicator must be coded as Unit of
    Analysis Code 3 (Sub-group level).

-   **Rule 7.1.3.3: Community Level (Code 4)**: If the Indicator Topic
    is Harvest volume and the final presentation of the indicator lists
    the total catch in the fishery overall, OR a summary statistic (like
    average or median) aggregated across all individual fishers in the
    defined fishery/community, the indicator must be coded as Unit of
    Analysis Code 4 (Community level).

## **7.2 Examples of Coding for Unit of Analysis**

| Indicator Topic | Variable Assessment Details                                                              | Final Presentation of Indicator                                 | Unit of Analysis Code | Unit of Analysis Description |
|---------------|---------------|---------------|:-------------:|---------------|
| Harvest volume  | Volume of catch by individual fishers by fishing trip                                    | Total volume of catch by each fisher                            |           1           | Individual level             |
| Harvest volume  | Volume of catch by individual fishers in a fishery characterized by multiple gear groups | Total harvest volume caught by fishers in a specific gear group |           3           | Sub-group level              |
| Harvest volume  | Volume of catch by individual fishers                                                    | Total catch in the fishery overall                              |           4           | Community level              |
| Harvest volume  | Volume of catch by individual fishers                                                    | Average catch per fisher                                        |           4           | Community level              |
| Harvest volume  | Expert estimate of total catch in a fishery                                              | Total catch in the fishery overall                              |           4           | Community level              |
| Harvest volume  | Expert estimate of total catch by gear group                                             | Total catch in the fishery overall                              |           4           | Community level              |
| Harvest volume  | Expert estimate of total catch in a fishery                                              | Total harvest volume across multiple distinct fisheries         |           6           | Supra-community level        |

# **8.0 Indicator Action**

The following typology should be used to select the best code for the
**Indicator Action** of the indicator:

|  Code   | Action                  | Definition                                                                                                                                                                                                                                      |
|:--------------------------:|:---------------------|:---------------------|
|  **1**  | **Evaluation**          | The indicator is being used in this study to evaluate a fishery (e.g., assessment or evaluation using information from a real fishery).                                                                                                         |
|  **2**  | **Development/testing** | This indicator is being developed or tested to support its future use in assessment or evaluation of a real-world fishery.                                                                                                                      |
|  **3**  | **Undetermined**        | Information is reported about the use of the indicator, but it is not clear whether Code #1 and/or Code #2 is relevant to this indicator.                                                                                                       |
| **n/r** | **Not reported**        | No information is reported in the source text regarding whether the indicator is being used for assessment/evaluation of a fishery and/or whether the indicator is being tested and refined to support its future use in assessment/evaluation. |

## **8.1 Special Rules for Indicator Action**

### **Rule 8.1.1 Non-Exclusivity (Evaluation and Development/Testing)**:

Codes 1 (Evaluation) and 2 (Development/testing) are not mutually
exclusive and may be applied simultaneously to the same indicator if the
study's narrative supports both actions. An indicator may be used to
evaluate a real fishery in the current study (Code 1) and may
simultaneously be the focus of methodological testing, refinement, or
initial development intended for future application (Code 2). If both
actions are documented, the final code for the indicator should be
recorded as "1; 2".

### **Rule 8.1.2 Action Cascade Rule**: If an indicator (Y) is coded as an Outcome Type Code 6, 7, 8, 10, or 11 then:

1.  **Direct Inputs Must Inherit**: All immediate constitutive
    sub-variables (X) listed in Y's Associated Sub-variable column
    (Table 2) must receive the same Indicator Action code(s) (Evaluation
    = Code 1; Development/testing = Code 2) as the associated outcome
    variable.
2.  **Transitivity**: This inheritance must cascade down the entire
    chain until a variable is reached that has an Outcome Type of n/r,
    5, 12, or a Basic Variable Type (1-4). (Example: If Composite Index
    $\text{C}$ (Output) is Code 2, and $\text{C} = \text{A} + \text{B}$,
    then both $\text{A}$ and $\text{B}$ must also be Code 2.)

# **9.0 Empirical vs Modeled (Data Source 1)**

The following typology should be used to select the best code for the
**Empirical vs Modeled (Data Source 1)** of the indicator:

|  Code   | Empirical vs Modeled (Data Source 1) Type | Definition                                                                                                                                                                                                                   | Special Instructions                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:-----------------:|:-----------------|:-----------------|:-----------------|
|  **1**  | **Empirical**                             | The indicator's assessed value is based directly on **real-world measured or collected data** (e.g., field measurements, survey results, baseline estimates, or descriptive statistics derived directly from measured data). | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Empirical** (Code 1) **ONLY if** all associated sub-variables received Code 1 in the Empirical vs. Modeled column.                                                                                                                                                                                                                      |
|  **2**  | **Modelled**                              | The indicator's assessed value is the **product or output of a complex mathematical or statistical simulation**, including dynamic system models (e.g., bio-economic, ecosystem dynamics, forecasting).                      | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Modeled** (Code 2) if one or more of its associated sub-variables received Code 2 in the Empirical vs. Modeled column. This rule ensures consistency with the Model Output inheritance rule described in the definition of Outcome Type code 10 (Model Output) in the section [3.2 Outcome Variable Types](#32-outcome-variable-types). |
|  **3**  | **Undetermined**                          | Information is reported about the indicator, but the distinction between an input (Empirical) source and a generative output (Modelled) source cannot be clearly established.                                                | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Undetermined** (Code 3) if a. no associated sub-variables are coded as "Modeled" (Code 2) and b. at least one associated sub-variable received the entry "undetermined" (Code 3) or "n/r" in the Empirical vs Modeled column.                                                                                                           |
| **n/r** | **Not reported**                          | No information is reported in the source text regarding whether the assessed value of the indicator is an input (Empirical) source and a generative output (Modelled) source.                                                |                                                                                                                                                                                                                                                                                                                                                                                                                                                           |

## **9.1 Special Rules for Empirical vs Modeled (Data Type 1)**

### **Rule 9.1.1 Outcome Type Symmetry Rule for Modeled Indicators**:

If the Outcome type for this indicator includes Code 10 (Model output)
from the Outcome Type typology in section [3.2 Outcome Variable
Types](#32-outcome-variable-types), the Data Type **must be
symmetrically coded as Modeled** (Code 2).

# **10.0 Primary vs Secondary (Data Source 2)**

The following typology should be used to select the best code for the
**Primary vs Secondary (Data Source 2)** of the indicator:

|  Code   | Primary vs Secondary (Data Source 2) Type | Definition                                                                                                                                                                                          | Special Instructions                                                                                                                                                                                                                                                                                                                                                                                                               |
|:-----------------:|:-----------------|:-----------------|:-----------------|
|  **1**  | **Primary**                               | The information used to assess/score this indicator was gathered through primary data collection).                                                                                                  | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Primary** (Code 1) **ONLY if** both the following conditions are met: a. all associated sub-variables received Code 1 in the Primary vs. Secondary column, and b. no associated sub-variables were modeled (Code 2 in the Empirical vs Modeled column).                                                          |
|  **2**  | **Secondary**                             | The information used to assess/score this indicator was drawn from previously existing data source(s).                                                                                              | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Secondary** (Code 2) **ONLY if** both of the following conditions are med: a. all associated sub-variables received Code 2 in the Primary vs. Secondary column and b. no associated sub-variables were modeled (Code 2 in the Empirical vs Modeled column).                                                      |
|  **3**  | **Statistically derived**                 | The indicator's assessed value is the product or output of a complex mathematical or statistical simulation, including dynamic system models (e.g., bio-economic, ecosystem dynamics, forecasting). |                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|  **4**  | **Undetermined**                          | Information is reported about the data source of the indicator, but the distinction between primary empirical data, secondary data, or statistically derived values cannot be clearly established.  | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Undetermined** (Code 4) if either of the following conditions is met: a. associated sub-variables received a combination of codes 1 and 2 in the column Primary vs Secondary, or b. at least one associated sub-variable received the entry "undetermined" (Code 4) or "n/r" in the Primary vs Secondary column. |
| **n/r** | **Not reported**                          | No information is reported in the source text regarding whether the assessed values of the indicator draws from primary empirical data, secondary data, or are statistically derived.               |                                                                                                                                                                                                                                                                                                                                                                                                                                    |

## **10.1 Special Rules for Primary vs Secondary (Data Source 2)**

### **Rule 10.1.1 Data Type Symmetry Rule (Statistically Derived)**:

If the **Empirical vs Modeled (Data Source 1)** column in section [9.0
Empirical vs Modeled (Data Source
1)](#90-empirical-vs-modeled-data-source-1) for this indicator is coded
as Modelled (Code 2), this Data Source 2 column must be symmetrically
coded as Statistically derived (Code 3).

### **Rule 10.1.2 Empirical Constraint**:

If the **Empirical vs Modeled (Data Source 1)** column in section [9.0
Empirical vs Modeled (Data Source
1)](#90-empirical-vs-modeled-data-source-1) for this indicator is coded
as Empirical (Code 1), the Data Source 2 column must be coded as either
Primary (Code 1) or Secondary (Code 2). It cannot be coded as
Statistically derived (Code 3).

## **10.2 Examples of Coding for Primary vs Secondary (Data Source 2)**

| Example                                                                                                                     | Primary vs Secondary (Data Source 2) Type | Correct Data Source 2 Code |
|--------------------|--------------------|:------------------------------:|
| Logbook with data recorded by fishers                                                                                       | Secondary                                 |             2              |
| Interviews with fishers about what they have recorded in their logbooks                                                     | Primary                                   |             1              |
| Responses to a survey instrument implemented for this specific study                                                        | Primary                                   |             1              |
| Responses to a survey instrument that was implemented for a previous study and the dataset is now being used for this study | Secondary                                 |             2              |
| Census data                                                                                                                 | Secondary                                 |             2              |
| Latent classes derived through latent class analysis                                                                        | Statistically derived                     |             3              |

# **11.0 Management Purpose Themes**

| Term                                  | Definition                                                                                                                                                                                                             |
|:-----------------------------------|:-----------------------------------|
| **Ambient monitoring**                | Systematic observation of the status of and changes in conditions over time.                                                                                                                                           |
| **Contextual or baseline assessment** | Documentation of the status of specific variables or conditions at a moment in time.                                                                                                                                   |
| **Historical analysis**               | Study of the past to understand ambient changes in specific conditions or the impacts of historical events, management activities, or interventions.                                                                   |
| **Impact assessment**                 | Rigorous and systematic assessment of the causal effects of a policy, program, project, activity, or investment.                                                                                                       |
| **Management evaluation**             | Measurement of the management inputs, activities, and outputs to assess strengths, weaknesses and needs.                                                                                                               |
| **Performance measurement**           | Measurement of implementation or progress toward specified project, program, or policy objectives, including inputs, activities, processes, outputs and outcomes.                                                      |
| **Predictive assessment**             | Application of future oriented methodologies (e.g., scenario planning, forecasting, structured decision-making) to identify and forecast the future impacts of potential interventions and deliberate on alternatives. |
| **Synthetic analysis**                | A structured and rigorous analysis of data from more than one case study or location or a meta-analysis of published studies to collate and synthesize empirical evidence and draw out broad lessons.                  |

# **12.0 Sustainability Themes**

| Term                              | Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|:-----------------------------------|:-----------------------------------|
| **General sustainability**        | This is a place to code variables noted to be "indicators of sustainability" broadly, without any further detail that would enable them to be assigned to a more specific sustainability theme sub-category. NOTE: "Sustainable development" and "Triple bottom line fisheries performance" are both considered to be synonyms for "sustainability" for the purposes of this systematic review.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Other sustainability theme**    | This is a place to code variables/indicator topics that fit seem to be a higher level sustainability theme, but are not represented in the current list of sustainability themes. Indicators coded to this will be reviewed to consider updates to the list of sustainability themes, whether in terms of definitions or in terms of adding new sub-categories.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Ecological sustainability**     | Also referred to as ecological performance, this is defined to include whether or not fisheries are environmentally non-degrading and allow for conservation of water, aquatic plants and animal genetic resources. Ecological sustainability entails maintaining individual stocks and species at levels that do not foreclose future options and maintain or enhance the capacity and quality of the ecosystem and environmental resources.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Economic sustainability**       | Also referred to as economic performance, this is defined to include economic viability, overall economic profitability over time, and equitable distribution of economic benefits. Economic sustainability focuses on the generation of sustainable benefits and maintains the economic welfare of fisheries, equitably distributing these benefits amongst participants, and maintaining overall viability within local and global economies.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Equality, equity, and justice** | Aspects of equality and equity consider equal and/or fair and just conditions and treatment of people, including in how laws and policies are developed and applied, as well as in their outcomes. Equality and equity are considered in terms of distribution (equality and/or fairness in outcomes and impacts of decision); procedure (equality and/or fairness in who is involved in decision-making and how decisions are made), and recognition (equality and/or fairness in how diverse values, knowledges, worldviews, and ways of life are acknowledged and legitimized). The aspect of justice considers structures that enable equality and equity.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Ethical sustainability**        | Ethical sustainability combines ecosystem justice -- preserving the intrinsic value and interconnectedness of all ecosystem members, realized through precautionary management, and social justice -- enabling just societies and institutions that value human rights, equality, and solidarity to participate in the utilization and conservation of fishery resources, realized through just management through participatory decision-making and collaborative governance. Ecosystem justice integrates productive justice and restorative justice, while social justice is defined to integrate distributive justice and retributive justice. Productive justice (an element of ecosystem justice) includes Ideal productive justice (Managing or stewarding the ecosystem and fishery resources to produce desired levels of benefits) and Realized productive justice (Adapting to environmental fluctuations and mitigating ecosystem depletion and habitat destruction). Restorative justice (an element of ecosystem justice) includes Ideal restorative justice (Restoring lost levels of benefits by rebuilding ecosystems, biodiversity and fishery resources) and Realized restorative justice (Limiting discards, wastes, and bycatch to maintain resilience and restoring ecosystems after damage caused by human actions). Distributive justice (an element of social justice) includes Ideal distributive justice (Sharing equitably the benefits from fishery resources within the ecosystem) and Realized distributive justice (Equity in entry and allocation, based on adjacency and reliance, and alternative livelihoods). Retributive justice (an element of social justice) includes Ideal retributive justice (Paying for the privilege to fish) and Realized retributive justice (Compensating for social and environmental costs of fishing, for example, harm, and penalizing IUU fishing).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Food security**                 | Studies aimed at evaluating whether fishers or fishing community members are meeting basic needs in terms of access to nutrition (and water), as well as studies aimed at identifying solutions and developing programs to support improvements in food security.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Institutional sustainability**  | Institutional sustainability is a prerequisite for [ecological, economic, and social] sustainability... It involves maintaining suitable financial, administrative and organizational capability in the longterm; the orientation of institutional change in such a manner as to ensure the attainment of continued satisfaction of human needs for present and future generations.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Job satisfaction**              | Studies framed around the idea of evaluating job satisfaction (this is highly intertwined with well-being research, but a distinct framing).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Poverty eradication**           | Studies aimed at understanding and mitigating the factors leading to poverty among fishers.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Resilience**                    | "Fisheries SES resilience; Fishing community resilience; Individual fisher resilience. Resilience broadly:"The term resilience has been conceptualized differently in various fields (Brand and Jax 2007, Martin-Breen and Anderies 2011). At its most basic, resilience is used in the field of engineering to refer to the ability of a material to resist external forces, shocks, and disturbances and to quickly return to its normal state (Martin-Breen and Anderies 2011). Furthermore, considering the context of individuals and their interactions with their families and larger communities, an individual's "psychological resilience" is defined as "a person's ability to use available resources to overcome stress and adversity" (Kirmayer et al. 2009:63)" (Himes-Cornell and Hoelting, 2015, p. 2). Fisheries SES: "Resilience is present in the concept of"persistence," the likelihood that an ecological system or SES will persist in its present stability domain rather than crossing a threshold into an alternative state (Holling and Gunderson 2002, Folke et al. 2010). However, this resilience framework also incorporates elements of adaptability, i.e., the capacity of actors in a system to influence resilience, and transformability, i.e., the capacity to create a fundamentally new system when ecological, economic, social, or political conditions make the existing system untenable (Walker et al. 2004). Considering persistability, adaptability, and transformability side by side allows for improved consideration of resilience overall, including human agency, power dynamics, justice, equality, and well-being within social systems (Davidson 2010, Folke et al. 2010, Coulthard 2012, Keck and Sakdapolrak 2013)" (Himes-Cornell and Hoelting, 2015, p. 2). Community resilience: "The resilience of a community as a social unit is dependent on the personal attributes and choices of the individuals that make up that community, as well as the ecological functioning of the SES. The well-being of individuals is impacted by the overall functioning of the community unit and SES, as well as opportunities available to them both locally and elsewhere. In the context of Alaskan fishing communities, the resilience of the overarching fishery SES depends on the persistability and adaptability of the community and the fishery resource base. Scholarship on community resilience has largely focused on the resources a community possesses, i.e.,"community capital," and the degree to which the community can collectively develop and engage these resources to improve well-being (Magis 2010)" (Himes-Cornell and Hoelting, 2015, p. 2). Individual resilience: The resources available to an individual may include personal traits, such as self-esteem, cognitive and problem-solving abilities, health, appearance, and temperament; social relationships, including the ability to seek comfort, support, and/or inspiration from other individuals; and personal beliefs, meaning, and self-knowledge (Kirmayer et al. 2009). Broad categories of community capital include the following: natural capital, i.e., natural resources and ecosystem services; social capital, i.e., relationships and connections between community members and between community members and the outside world; cultural capital, i.e., shared traditions, beliefs, and values that increase social cohesion; human capital, i.e., the skill sets and knowledge base of the population that can contribute to creative problem solving; political capital, i.e., the presence of functioning institutions and the ability of community members to influence the outcome of decisions that affect them; built capital, i.e., infrastructure and other physical resources in the community; and financial capital, i.e., assets and access to financing mechanisms (Emery and Flora 2006, Rolfe 2006, Kirmayer et al. 2009, Magis 2010). An individual's personal resilience strategy has the potential to increase community resilience if he/she has resources to add to the community's capital. However, an individual's personal resilience strategy may involve migration when opportunities are not available locally or when opportunities in other locations are more attractive. In such cases, resilience at the individual level has the potential to undermine community resilience through contributing to overall population decline and loss of the resources an individual contributes to the larger community. Given this, resilience at one level of a system may not correlate to resilience at another level (Marshall et al. 2007, Robards and Greenberg 2007, Kirmayer et al. 2009)" (Himes-Cornell and Hoelting, 2015, p. 2)." |
| **Social responsibility**         | A framework of ethical guidelines and principles for fisheries management and research / conservation initiatives. This includes studies focused on corporate social responsibility.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Social sustainability**         | Also referred to as social performance, this sustainability theme includes higher-level conceptual indicators related to the social acceptability of fishing activities, in terms of ensuring fisheries lead to 'social profitability' in the sense of social cost-benefit analysis, and also that fisheries regulations support well-being of fishers and fishing communities. Social sustainability focuses on well-being at the group level, recognizing the fishermen as a community rather than a collection of individuals. Hence, emphasis is on maintaining or enhancing the group welfare of participating and affected communities, including economic and sociocultural welfare, overall cohesiveness and the long-term health of the human system.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Sustainable livelihood**        | Livelihood stability, resilience, and improvement. This is imagined to be accomplished through: 1) developing social and human capital in communities; 2) maintaining or enhancing natural assets; 3) supporting development of appropriate policy and institutional environments.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Technological sustainability**  | Technological sustainability involves the appropriate use of technology in order that minimizes risks to the sustainable development of fisheries and eliminates any negative effects on the environment or ecology caused by fishing. It is the orientation of technological change in such a manner as to ensure the attainment of continued satisfaction of human needs for present and future generations.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Well-being**                    | Studies aimed at evaluating community well-being, or individual well-being, including focus on subjective and/or objective well-being of fishers or fishing communities.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

# **13.0 Conceptual Categories**

For each indicator identified by the AI, I would like the AI to
determine the concept of the variable being assessed -- the **variable
concept** -- with reference to a set of conceptual categories. In
addition, I would like the AI to determine whether the overarching
indicator is being used to indicate the same concept that the variable
is assessing, or if the **indicator topic** is in fact conceptually
distinct from the variable concept. In such cases, a **conceptual
proxy** is present in the construction of the indicator, as described in
section [14.1.3 Conceptual proxy](#1413-conceptual-proxy). This means
that a variable of one concept is being used as the basis for an
indicator that is representing a distinct concept. For example, the
variable may assess income levels of fishers, but the indicator may be
intended to represent food security of fishers. Because it is possible
that the variable concept is distinct from the concept of the indicator
topic, I will ask the AI to identify both the variable concept and the
indicator topic and to match each to the best conceptual category. If
the variable concept and indicator topic are the same, both will be
coded to the same category.

**Indicator Topic Conceptual Scope Constraint**: The **Indicator Topic**
(the **conceptual representation target**) must be matched to a concept
within a specific Primary Category (see section [13.2 Primary Category
Definitions](#132-primary-category-definitions)) and Sub-category (see
section [13.3 Sub-category definitions](#133-sub-category-definitions)).
The sole exception is when authors explicitly design an indicator to
assess a high-level conceptual theme, such as "sustainability" writ
large; only in these rare cases should the Indicator Topic be coded to a
sub-category within the **Larger sustainability theme** Primary
Category. The standard, targeted concepts in the framework (e.g.,
Harvest characteristics, Material benefits, Rule of law) must be
prioritized over high-level sustainability themes, even if the indicator
is noted as "contributing to" a sustainability theme.

## **13.1 Process for matching a concept to a sub-category**

```         
1. **Select primary category**: The first step in determining the appropriate **sub-category** to code the variable concept and the indicator topic is to identify which **primary category** is the best conceptual location, i.e., does the indicator have to do with fishery participant well-being (capabilities, conditions, or connections), fishery governance (characteristics or performance), the fishery system (characteristics or performance, including economic, environmental, and social performance), or context (environmental context, human dimensions context, or community context). Definitions for each primary category are provided in the section [13.2 Primary Category Definitions](#13.2-primary-category-definitions).

2. **Select sub-category within the chosen primary category**: The second step in determining the appropriate sub-category to code the variable concept and the indicator topic is to identify the best sub-category within the selected primary category. Sub-category definitions are provided in the section [13.3 Sub-Category Definitions](#13.3-sub-category-definitions).
```

### **13.1.1 Notes and Special Rules for Sub-category Selection**:

-   **General and Other Sub-categories**: "General" and "Other"
    sub-categories exist within each primary category. These are
    included in the event that either: a. AI can identify the
    appropriate primary category, but no sub-category offers the correct
    conceptual fit (in which case AI must code to the "Other"
    sub-category within the selected primary category), or b. the
    variable concept or indicator topic spans more than one conceptual
    sub-category within the selected primary category (in which case AI
    must code to the "General" sub-category within the selected primary
    category).
-   **Examples Provided in Definitions are Not Exhaustive**: The
    existing definitions of primary categories and sub-categories
    currently include various examples to help AI locate the best-fit
    sub-category for a given variable concept or indicator topic, but
    the examples listed in the definitions are not exhaustive. **If the
    AI notices that a definition is a good fit in general, but the
    specific example of the variable concept or indicator topic is not
    reflected in the existing definition, AI must flag the example as a
    recommended addition to the definition. AI must also recommend
    adjustments to primary category or sub-category definitions if AI
    notices inconsistencies within a single definition or unnecessary
    conceptual overlaps between definitions of multiple categories.**
-   **Use Full Sub-Category Name**: In the Table outputs, when
    identifying the best sub-category for an indicator's **variable
    concept** or an indicator's **indicator topic**, the AI **must
    indicate the sub-category name word for word.**

## **13.2 Primary Category Definitions**
                                                                                                            
FAO's primary conceptual categories have been redacted from this version of the GIP. FAO is in the process of finalizing their conceptual classification system. Once category definitions have been finalized this GIP will be updated with primary category names and definitions that AI can use to carry out conceptual coding of identified indicators.

## **13.3 Sub-category Definitions**
                                                                                                            
FAO's conceptual sub-category definitions have been redacted from this version of the GIP. FAO is in the process of finalizing their conceptual classification system. Once category definitions have been finalized this GIP will be updated with primary category names and definitions that AI can use to carry out conceptual coding of identified indicators.

# **14.0 Relationships Within and Between Indicators**

I am interested to track several types of conceptual relationships that
exist both within the description of a single indicator, and between two
distinct indicators included in AI's list of relevant indicators.

-   **Within-Indicator Relationships**: The types of within-indicator
    relationships of interest include:

    -   **Conceptual Proxy**: The **primary variable concept** is used
        as a proxy for the **indicator topic**. Definitions are provided
        in section [14.1.1 Conceptual Elements within a Single
        Indicator](#1411-conceptual-elements-within-a-single-indicator),
        and the protocol for identifying presence or absence of a
        conceptual proxy is provided in section [14.1.3 Conceptual
        proxy](#1413-conceptual-proxy).
    -   **Secondary Variable Concepts**: After identifying the **primary
        variable concept**, i.e., the primary conceptual assessment
        target of the variable, there may be additional, **secondary
        variable concept(s)** described in the **indicator definition**
        and/or **variable assessment details**. The conceptual
        sub-category of these secondary concepts must also be recorded
        in Table 3 following definitions provided in section [14.1.1
        Conceptual Elements within a Single
        Indicator](#1411-conceptual-elements-within-a-single-indicator)
        and protocols outlined in section [14.1.2 Protocols for
        Identifying Conceptual Components Within
        Indicators](#1412-protocols-for-identifying-conceptual-components-within-indicators].

-   **Between-Indicator Relationships**: The types of between-indicator
    relationships of interest include:

    -   **Sub-variables and Outcome Variables**: The role of some
        indicators as constitutive **sub-variables** used to calculate
        other **outcome variable** indicators (see section [14.2
        Sub-variables and Outcome
        Variables](#142-sub-variables-and-outcome-variables)
    -   **Relating variables and Target Variables**: The role of one
        indicator (X) as a **relating variable** and another indicator
        (Y) as a **target variable**. The terms relating variable and
            target variable are broad terms used to capture concepts
            such as predictor and response variables, independent and
            dependent variables, as well as types of X-Y relationships
            that are not directional or not statistically explored.
            Definitions of types of X-Y relationships are provided in
            section [14.3 X-Y relationship
            types](#143-x-y-relationship-types).

## **14.1 Within-Indicator Conceptual Relationships**

### **14.1.1 Conceptual Elements within a Single Indicator**

If all three **basic variable components** are reported in the study
(Indicator Name, Indicator Definition, and Variable Assessment Details),
as described in section [2.0 Instructions for Identifying Relevant
Indicators](#20-instructions-for-identifying-relevant-indicators), it
will be possible to discern all of the **conceptual elements** for the
indicator. If the Variable Assessment Details are not provided in the
study, it will only be possible to identify the Indicator Topic. The
full set of conceptual elements are as follows:

| Conceptual Component                      | Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Protocol Reference |
|:-----------------------|:-----------------------|:-----------------------|
| **Indicator topic**                       | The **conceptual representation target** (the goal concept). Always present. [MANDATE for Sub-variables]: For any indicator acting as a $\mathbf{Sub-variable}$ to a **Composite index** (Code 4 in Table 4) or an **Other derived outcome** (Code 5 in Table 4), the Indicator Topic MUST be conceptually identical to the Primary Variable Concept unless the original source text explicitly states that the sub-variable is used as a proxy for an external concept. The only exception is for inputs to Latent Constructs (Code 7 in Table 4), where the IT of the sub-variable defaults to the IT of the Latent Construct. The Indicator topic is always present. | Protocol 14.1.2.1  |
| **Primary Variable Concept**              | The **primary conceptual assessment target** (the concept being directly assessed). Present if Variable Assessment Details are available.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Protocol 14.1.2.4  |
| **Specifying Secondary Variable Concept** | A **more specific conceptual component** used to detail a general Primary Variable Concept.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Protocol 14.1.2.5  |
| **Equation Secondary Variable Concept**   | A **conceptual sub-variable** implied by the indicator's mathematical structure or indicator definition but not fully described in the study as a stand-alone sub-variable.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Protocol 14.1.2.6  |
| **Predictor Secondary Variable Concept**  | A **conceptual element described as influencing or correlating** with the Indicator Topic/Primary Variable Concept within the indicator's definition.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Protocol 14.1.2.7  |

### **14.1.2 Protocols for Identifying Conceptual Components Within Indicators**

#### **14.1.2.1 Format Constraint: Multiplicity of Secondary Concepts**:

The following rule applies to all subsequent protocols having to do with
identification of **Secondary Variable Concepts** (Protocols 14.1.2.6,
14.1.2.7, and 14.1.2.8):

**Multiplicity Format Constraint**: If an indicator description yields
more than one secondary variable concept (Specifying, Equation, or
Predictor), the corresponding conceptual sub-categories and definition
matches reported in Table 3 **must be separated by a semi-colon (;) for
each distinct entry.** (Example: "Material benefits; Food security and
consumption").

#### **14.1.2.2 Protocol for Indicator Topic Assignment for Sub-variables**:

The **Indicator Topic** assignment for any indicator that also serves as
a **Sub-variable** of a complex aggregate (Relational Codes 3, 4, or 5
in Table 6) must follow this precedence: 1. **Default Rule**: The
Indicator Topic must be conceptually identical to the
$\mathbf{Primary \ Variable \ Concept}$ (i.e., the sub-variable is its
own topic). This results in Proxy Absent (n/a). 2. **Explicit Proxy
Exception**: Override the default rule only if the source text
explicitly names the sub-variable (X) as a measure of a distinct,
high-level concept (Z) not equal to the Primary Variable Concept.
(Resulting in Proxy Present (Yes)).

#### **14.1.2.3 Protocol for Latent Construct Sub-variables (Code 7 Exception)**:

If the indicator acts as a $\mathbf{Sub-variable}$ feeding into a
$\mathbf{Latent \ Construct \ (Code \ 7)}$ output, the **Indicator
Topic** $\mathbf{MUST}$ be the name/concept of the Latent Construct
itself. This reflects the conceptualization that the sub-variable is an
observable manifestation of the latent construct, thereby acting as a
proxy for it (resulting in Proxy Present (Yes) if categories are
distinct, or Proxy Absent (n/a) if the construct name happens to map to
the same category).

#### **14.1.2.4 Protocol for Identifying Indicator Topic**

The Indicator Topic is the conceptual representation target of the
indicator and is always present. It must be discerned based on a
comprehensive review of all available basic indicator components
(Indicator Name, Indicator Definition, and/or Variable Assessment
Details).

-   **Discretion Rule**: If only one basic indicator component is
    available, the indicator topic must be discerned based solely on
    that one component

#### 14.1.2.5 Protocol for Identifying the Primary Variable Concept\*\*

The Primary Variable Concept is the primary conceptual assessment target
of the indicator. Its identification is strictly conditional on the
study providing details on how the variable was assessed.

-   **Condition**: This element is possible to discern and always
    present if and only if Variable Assessment Details are provided for
    the indicator in the source text.
-   **Discernment**: The Primary Variable Concept must match the main
    concept of the indicator that is directly being measured or
    assessed.

#### **14.1.2.6 Protocol for Identifying a Specifying Secondary Variable Concept**

-   **Trigger**: Indicator definition or Variable Assessment Details are
    present.

-   **Step 1 (Check Scope)**: Does the variable description contain both
    a general conceptual component and a specific conceptual component?

-   **Step 2 (Check Conceptual Match)**: Do the general and specific
    components match to distinct conceptual sub-categories?

-   **Step 3 (Execution)**: If the condition in Step 2 is Yes, the AI
    must report the following information in Table 3:

    a.  **Secondary variable concept type**: Begin each entry with the
        type of secondary variable element, followed by colon space
        (":"), (e.g., "Specifying:").
    b.  **Secondary Concept**: Report the specifying concept (e.g.,
        "Catching power of gear"), followed by comma space (","). For
        example, if an indicator has the **primary variable concept** of
        "Catching power", and the indicator definition and/or variable
        assessment details clarify that the indicator is specifically
        about a particular aspect or type of catching power, e.g.,
        catching power of the gear (as opposed to the vessel itself or
        the number of crew), AI should recognize the presence of a more
        specific concept beyond catching power, and enter the more
        specific concept "Catching power of harvest gear,".
    c.  **Associated Sub-category**: Report the conceptual sub-category
        that best matches the implied concept (e.g., "Harvest gear").
        (Reference definitions in section [13.3 Sub-category
        definitions](#133-sub-category-definitions)).
    d.  **Multiplicity**: If several specifying conceptual elements are
        implied by the definition and/or variable assessment details,
        separate individual entries using a semi-colon and space (";").
        If other types of secondary variable concepts are also listed,
        these must also be separated by a semi-colon and space (";").

#### **14.1.2.7 Protocol for Identifying an Equation Secondary Variable Concept**

-   **Trigger**: The **indicator definition** and/or **Variable
    Assessment Details** are present.

-   **Step 1a (Check Calculation Logic)**: Does the variable assessment
    description suggest conceptual elements that were used to calculate
    or structurally define the Indicator Topic?

-   **Step 1b (Mandate for Code 11 Constitutive Elements)**: For any
    indicator whose Outcome Type is Categorical Outcome (Code 11), the
    conceptual characteristics/sub-variables that define the grouping
    (e.g., economic capacity, regulatory environment, geographic
    location) MUST be treated as Equation Secondary Variable Concepts
    and documented following Step 2, even if no arithmetic calculation
    is present.

-   **Step 2 (Execution)**: If the condition in **Step 1a is Yes** OR if
    the mandate in **Step 1b applies**, the AI must report the following
    information in Table 3:

    a.  **Secondary variable concept type**: Begin each entry with the
        type of secondary variable element, followed by colon space
        (":"), (e.g., "Equation:").
    b.  **Secondary Concept**: Report the concept being structurally
        implied (e.g., "Days at sea"), followed by comma space (",").
        For example, if an indicator with the **indicator topic**
        "Fishing effort", and the indicator definition and/or variable
        assessment details suggest that one of the elements of the
        calculation involved the number of days at sea, AI should
        recognize this as an equation secondary variable element that is
        structurally constitutive of the indicator topic, and enter
        "Days at sea,".
    c.  **Associated Sub-category**: Report the conceptual sub-category
        that best matches the implied concept (e.g., "Harvest
        practices"). (Reference definitions in section [13.3
        Sub-category definitions](#133-sub-category-definitions)).
    d.  **Multiplicity**: If several equation conceptual elements are
        implied by the definition and/or variable assessment details,
        separate individual entries using a semi-colon and space (";").
        If other types of secondary variable concepts are also listed,
        these must also be separated by a semi-colon and space (";").

#### **14.1.2.8 Protocol for Identifying a Predictor Secondary Variable Concept**

-   **Trigger**: Indicator definition or Variable Assessment Details are
    present.

-   **Step 1 (Check Relationship)**: Is a directional or non-directional
    relationship between conceptual elements described within the
    indicator's definition/details?

-   **Step 2 (Execution)**: If the condition in Step 1 is Yes, the AI
    must report the following information in Table 3:

    a.  **Secondary variable concept type**: Begin each entry with the
        type of secondary variable element followed by the type of X-Y
        relationship present (using the X-Y relationship typology in
        section [14.3.2 X-Y Relationships to
        Record](#1432-x-y-relationships-to-record)), followed by colon
        space (":"), (e.g., "Predictor5:").
    b.  **Secondary Concept**: Report the concept acting as a relating
        variable (X) for the primary variable concept (Y), followed by
        comma space (","). For example, if the primary variable concept
        of an indicator % active fishing permits, and the definition of
        the variable is "the effect of fuel costs on the proportion of
        fishing permits that are actively fished," AI should recognize a
        relating variable, "Cost of Fuel" (X) acting on the primary
        variable concept and enter "Cost of Fuel," as a predictor
        secondary concept.
    c.  **Associated Sub-category**: Report the conceptual sub-category
        that best matches the implied concept (e.g., "Variable costs").
        (Reference definitions in section [13.3 Sub-category
        definitions](#133-sub-category-definitions)).
    d.  **Multiplicity**: If several predictor conceptual elements are
        implied by the definition and/or variable assessment details,
        separate individual entries using a semi-colon and space (";").
        If other types of secondary variable concepts are also listed,
        these must also be separated by a semi-colon and space (";").

### **14.1.3 Conceptual proxy**

The **Primary Variable Concept** and the **Indicator Topic**, as defined
in section [14.1.1 Conceptual Elements within a Single
Indicator](#1411-conceptual-elements-within-a-single-indicator), are two
conceptual components of an indicator. The AI must use the following
steps to identify whether or not a **conceptual proxy** is present
between the primary variable concept and the indicator topic:

| Step                   | Action and Condition                                                                                                                                                                                        |
|:-----------------------------------|:-----------------------------------|
| **Trigger**            | Both the **Primary Variable Concept** and the **Indicator Topic** have been successfully matched to a conceptual sub-category (following section [13.0 Conceptual categories](#130-conceptual-categories)). |
| **Step 2 (Execution)** | Determine the status and apply the output in the appropriate column (Conceptual Proxy Present):                                                                                                             |
|                        | **a. Proxy Absent (Direct Measure):** If the two conceptual sub-category assignments are **IDENTICAL**, the variable is a direct measure and no conceptual proxy is present.                                |
|                        | **b. Proxy Present (Indirect Measure):** If the two conceptual sub-category assignments are **DISTINCT**, a conceptual proxy is present (e.g., using income to represent food security).                    |

## **14.2 Sub-variables and Outcome Variables**

I would like the AI to make note when one indicator serves as a
sub-variable in the calculation of another indicator in the list of
relevant indicators. Later when the AI produces a table with each
indicator and its associated attributes, one attribute column will be
dedicated to cross-referencing associated outcome variables (if the
indicator acts as a sub-variable), and one column will be dedicated to
cross-referencing associated sub-variables (if the indicator is an
outcome variable built from sub-variables). The rules guiding this
process are described in sections [14.2.1 Preparatory Mandates (Defining
the Data Set)](#1421-preparatory-mandates-defining-the-data-set),
[14.2.2 Immediate Constitutive Link Rule (Defining the Structural
Requirements)](#1422-immediate-constitutive-link-rule-defining-the-structural-requirements),
and [14.2.3 Verification and Execution Protocols (Ensuring
Accuracy)](#1423-verification-and-execution-protocols-ensuring-accuray).

### **14.2.1 Preparatory Mandates (Defining the Data Set)**:

These rules ensure all necessary components of the constitutive
hierarchy are included as discrete indicators before mapping begins:

1.  **Constitutive Term Inclusion Mandate**: The AI \*\*must ensure that
    any component (X) used to determine the value of an outcome variable

    (Y) is separately identified and included as its own unique
        indicator.\*\* This mandate applies regardless of the conceptual
        relationship type:

    -   **Constitutive Building Blocks**: Sub-variables that are
        synthesized or aggregated to define a multifaceted concept
        (e.g., inputs for Code 6).
    -   **Observable Manifestations**: Individual metrics used as
        reflective indicators to estimate an unobservable latent state
        (e.g., inputs for Code 7).
    -   **Functional/Structural Components**: Variables used in
        mathematical transformations, ratios, or structural tallies of
        related units (e.g., inputs for Code 8).
    -   **Identifying Attributes**: Characteristics used as criteria to
        assign a typological identity or regime (e.g., inputs for Code
        11).

2.  **Standard Aggregate Decomposition Protocol (SADP)**: When applying
    the Immediate Constitutive Link Rule to complex aggregate variables,
    the AI **must use a strict one-step decomposition**:

    -   **Aggregate Inputs**: If an indicator (A) is defined by a
        formula listing multiple sub-aggregate variables (e.g., A = B +
        C + D), the immediate, one-step inputs (Associated Sub-variables
        of A) are ONLY B, C, and D. The AI must not trace the
        relationship further back to the inputs of B, C, or D within the
        same row.
    -   **Conceptual Integrity**: This "one-step" rule applies to all
        aggregates, including Latent Constructs (Code 7) and Categorical
        Outcomes (Code 11). The AI must only link to the immediate
        attributes or manifestations described by the author, strictly
        upholding the **Hierarchical Precision and Redundancy Check
        (HPRC)**.

### **14.2.2 Immediate Constitutive Link Rule (Defining the Structural Requirements)**

These rules establish the definitive one-step standard for all links
documented in the columns and the resulting structural symmetry.

1.  **Immediate Constitutive Link (One-Step Constitutive Rule)**: The
    population of the Associated Outcome Variable and Associated
    Sub-variable columns must adhere to a strict one-step standard.

    a.  **Associated Outcome Variable**: An indicator (X) may only list
        an outcome variable (Y) if X is a direct and immediate input
        used in the mathematical calculation of Y.
    b.  **Associated Sub-variable**: An indicator (Y) may only list a
        sub-variable (X) if X is a direct and immediate input used in
        the calculation of Y.

    > **Decomposition Hierarchy Rule**: When an indicator is part of a
    > multi-level hierarchy (e.g., Variable A + Variable B = Sub-index
    > X; Sub-index X + Sub-index Y = Final Index Z), the AI **must stop
    > tracing at the first available intermediate node**. In this
    > example, the sub-variables for Final Index Z are ONLY Sub-index X
    > and Sub-index Y. The AI must NOT list Variable A or B as
    > sub-variables for Z. This ensures the data chain is mapped as a
    > sequence of discrete, single-step mathematical dependencies and
    > prevents double-counting across the hierarchy.

2.  **Constitutive Symmetry Rule**: For any direct, immediate
    constitutive relationship between a Sub-variable (X) and an Outcome
    Variable (Y), **the relationship must be coded symmetrically across
    the two indicator rows**, as follows: If X lists Y's number in its
    Associated Outcome Variable column, then... Y must list X's number
    in its Associated Sub-variable column.

3.  **Structural vs. Predictive Link Mandate (Classification of X**
    $\to$ Y Relationship): The directional relationship between an
    $\mathbf{Input \ Variable \ (X)}$ and its
    $\mathbf{Output \ Variable \ (Y)}$ must be classified based on
    $\mathbf{structural}$ or $\mathbf{causal}$ functionality to
    determine its mapping location: 1. **Constitutive Functionality**:
    If the Output Variable $\mathbf{(Y)}$ is coded as
    $\mathbf{Code \ 6, 7, 8, 10, \ or \ 11}$, the relationship must be
    mapped as a **Sub-variable** $\to$ Outcome Variable link. These are
    exclusively tracked in the Associated Columns (Table 2) and the
    Constitutive Flow Chart (P25). 2. **Predictive Functionality**: If
    the Output Variable $\mathbf{(Y)}$ is coded as $\mathbf{Code \ 12}$
    (Narrative Causal Outcome), the relationship must be mapped as a
    **Relating Variable** $\to$ Target Variable link. These are
    exclusively tracked in the Predictive Columns (Table 2) and the
    Predictive Flow Chart (P26).

### **14.2.3 Verification and Execution Protocols (Ensuring Accuracy)**

These rules define the mandatory order of execution to prevent
directional errors and enforce consistency.

1.  **Constitutive Link Directional Verification (CLDV)**: To ensure
    strict adherence to the Immediate Constitutive Link Rule, the AI
    must first prioritize identifying all relationships by their direct
    flow: Sub-variable (Input)  Outcome Variable (Output). To
    accomplish this, following these rules:

    a.  **Input Linkage Priority (Associated Sub-variable Column -\>
        Associated Outcome Variable Column)**: For any Indicator (A)
        that is an Outcome Variable, the AI **must definitively list all
        its one-step inputs in the Associated Sub-variable Column
        first**, using the relevant formula.

    b.  **Symmetry Enforcement (Associated Outcome Variable Column)**:
        Only after the Associated Sub-variable Column for Indicator A is
        complete, the AI **must populate the Associated Outcome Variable
        column for each of Indicator A's sub-variables, ensuring a
        symmetric cross-reference** (i.e., if Indicator B is in
        Indicator A's Associated Sub-variable Column, then Indicator A
        must be in Indicator B's Associated Outcome Variable Column).

    c.  **Prohibited Entries Check**: The AI **must perform a final
        check on the Associated Outcome Variable Column of every Outcome
        Variable (Indicator A) and confirm that Indicator B's column
        does not contain the indicator numbers of its own inputs**
        (which would violate the rule and signal a reversal of flow
        logic).

## **14.3 X-Y Relationship Types**

I would like the AI to record a spectrum of relationships between an X
variable (i.e., a **relating variable**) and a Y variable (i.e., a
**target variable**), other than the structural relationship between
sub-variables that structurally constitute a calculated outcome variable
or a categorical outcome variable. The section [14.3.1 X-Y Relationship
Exclusion and Inclusion
Rules](#1431-x-y-relationship-exclusion-and-inclusion-rules) explains
the type of structural X-Y relationship that AI should exclude from this
portion of attribute identification because it has separately been
captured in the relationship between sub-variables and outcome
variables, as directed in section [14.2 Sub-variables and Outcome
Variables](#142-sub-variables-and-outcome-variables). The section
[14.3.2 X-Y Relationship to Record](#1432-x-y-relationships-to-record)
provides definitions of the types of X-Y relationships that AI must
distinguish and record in this potion of attribute identification. The
following table lists key conceptual elements involved in X-Y
relationships in this section:

| Term                                 | Definition                                                                                                                                                                                                                                              | Relationship Role       | GIP Code Link                                                                                 |
|:-----------------|:-----------------|:-----------------|:-----------------|
| **Relating Variable (X)**            | The indicator serving as the independent variable or predictor. This encompasses the Narrative Causal Element (NCE) and any quantitative causal input.                                                                                                  | Input (Cause/Driver)    | N/A                                                                                           |
| **Target Variable (Y)**              | The indicator serving as the dependent variable or outcome that is being influenced. This encompasses the Narrative Causal Outcome (NCO) and any quantitative effect variable.                                                                          | Output (Effect/Outcome) | N/A                                                                                           |
| **Narrative Causal Statement (NCS)** | A directional relationship (X → Y) asserted by the research authors or study participants, derived from qualitative analysis (e.g., interviews, thematic coding). The statement links a Narrative Causal Element (X) to a Narrative Causal Outcome (Y). | Systemic/Predictive     | Code 5 (X-Y Relationship Type)                                                                |
| **Narrative Causal Element (NCE)**   | The **input or causal factor** (X) identified in an NCS. This variable is the **Relating Variable (X)** in the predictive analysis columns.                                                                                                             | Input (Cause)           | Code 4 (Basic Variable Type)                                                                  |
| **Narrative Causal Outcome (NCO)**   | The **output or effect** (Y) identified in an NCS. This variable is the **Target Variable (Y)** in the predictive analysis columns.                                                                                                                     | Output (Effect)         | Code 4 (Variable Type Upon Scoring); Code 12 (Outcome Type); Code 4 (Variable Type of Outcome |

### **14.3.1 X-Y Relationship Exclusion and Inclusion Rules**

The following rules guide the process of identifying relevant X-Y
relationships:

1.  **Structural Identity Exclusion Rule (The Definitional Test)**: The
    AI **must not** record an X-Y relationship (Codes 1-9) if the
    relationship is already captured as a structural, constitutive link
    as described in section [14.2 Sub-variables and Outcome
    Variables](#142-sub-variables-and-outcome-variables), **UNLESS that
    constitutive link is also explicitly identified as fulfilling a
    Causal-Testing Role (Rule 14.3.1.3)**. This exclusion applies when
    the model relationship defines an aggregate quantity, value, status,
    or classification, including all relationships involving:

-   **Simple Arithmetic Identity (Code 8)**: Relationships involving
    only simple arithmetic (summation, averaging,
    multiplication/division, ratio, or subtraction) used to define an
    aggregate quantity or value (e.g., Revenue = Price × Quantity; Total
    = Σ Parts).
-   **Status-Ranking Identity (Code 6)**: The definitional step of
    converting constitutive sub-variable scores into a performance-based
    status or rank (e.g., binning a numeric score into "High," "Medium,"
    or "Low" vulnerability). Because the purpose of the output is to
    represent the aggregate status of the multifaceted concept, it is a
    structural aggregation, not a systemic causal prediction.
-   **Manifestation Identity (Code 7)**: The reflective relationship
    where indicators are hypothesized to manifest an unobservable latent
    state (e.g., survey questions manifesting "Social Capital").
-   **Categorical Classification Identity (Code 11)**: The definitional
    step of assigning an identity or "type" based on a specific
    configuration of attributes (e.g., defining a "Fleet Segment" or
    "Management Regime" based on a specific combination of gear and
    vessel size).

This rule reserves the X-Y Predictive analysis for **Systemic
Causality** (non-definitional, high-level, or statistically tested
relationships). The precedence rule is enforced by the Causal-Testing
Priority Mandate (Rule 14.3.1.4).

2.  **External Predictive Role Mandate**: An indicator (X) whose primary
    role is to act as an Associated Sub-variable in a constitutive
    relationship (Codes 3, 4, or 5) **must still be recorded as a
    Relating Variable (X)** in the predictive columns if the study
    explicitly uses it as a predictor in a **separate, non-constitutive
    X-Y analysis**. This ensures that the indicator's **full systemic
    role**---both as a component (constitutive) and as a driver
    (predictive)---is documented, regardless of its position in a
    calculation chain.

3.  **Statistical Causal Inclusion Mandate (The Estimation Test)**:
    Notwithstanding Rule 1, the AI **must include** an X-Y relationship
    (Codes 1-9) if the link between X and Y is defined by a
    **statistically estimated parameter or coefficient** that was
    quantified through a model-fitting process (e.g., maximizing
    likelihood, minimizing errors, nonlinear regression). This mandate
    ensures that all relationships where the study's scientific purpose
    is to **test or quantify a hypothesized causal influence** (e.g.,
    calculating price flexibilities, regression coefficients) are
    documented in the **Relating variable** and **Target variable**
    columns.

4.  **Causal-Testing Priority Mandate**: When a relationship satisfies
    both the **Structural Identity Exclusion Rule (14.3.1.1)** and the
    **Statistical Causal Inclusion Mandate (14.3.1.3)**, the
    Causal-Testing role **MUST** take precedence for inclusion in the
    predictive columns. The link must be classified as **Constitutive
    and Predictive (Rule 3)** in the Rationale column.

**Application Note**: This applies specifically to cases where an
aggregate variable (Code 6 or 11) is not merely a sum of its parts, but
is used in a model-fitting process (e.g., sensitivity analysis,
regression) to quantify the specific influence of an input on the
outcome. In such cases, the relationship serves a dual role: 1. It
structurally defines the output (Constitutive), and 2. It scientifically
tests a causal hypothesis (Predictive).

### **14.3.2 X-Y Relationships to Record**

For any X-Y relationship that is not excluded based on the X-Y Exclusion
Rule, **the AI must record the type of X-Y relationships based on two
characteristics**: 1. Whether the X-Y relationship is directional or
non-directional, and 2. Whether evidence of the X-Y relationship is
statistical or non-statistical. Later, when the AI produces a table, the
numeric codes should be used as part of reporting the relating variable
to indicate the type of relationship between an X and Y variable. **The
output must be the numerical identifier (1 through 9) corresponding to
the following typology, not the text description:**

**Mandatory Two-Step X-Y Relationship Verification Protocol**: When
assigning a relationship code (1 through 9), the AI must follow this
strict two-step verification to ensure accuracy: 1. **Step 1: Role and
Directionality Mapping**: Identify whether the relationship is (a)
Directional (X $\to$ Y; hypothesis/model explicitly tests X's influence
on Y) or Non-Directional (X $\leftrightarrow$ Y; hypothesis/model tests
simple association/correlation). Concurrently determine the Statistical
Basis (Statistical, Non-Statistical, or Unknown). 2. **Step 2:
Significance Check**: If the relationship is found to be Statistical,
determine the outcome based on the reported $p$-value or equivalent
metric ($\alpha = 0.05$): Significant, Not Significant, or Unknown/Not
Reported. The final Code (1--9) must align precisely with the
combination of Directionality and Significance status defined in the
table below.

| Code  | Term                                                   | Full Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:--------------------------:|:---------------------|:---------------------|
| **1** | **Directional, statistical, significant**              | a directional relationship (influence of a relating variable on a target variable) was found to be statistically significant, e.g., regression analysis, sensitivity analyses, or other approaches to assessing the magnitude of effect of a single variable in a model, e.g., Cohen's d, the Phi ($\phi$) coefficient, or Cramér's V Regression;                                                                                                                                                                                                                    |
| **2** | **Directional, statistical, not significant**          | a directional relationship (influence of a relating variable on a target variable) was found NOT to be significant;                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **3** | **Directional, statistical, unknown significance**     | a directional relationship was present (influence of a relating variable on a target variable), but the significance of the relationship was not reported or was undetermined;                                                                                                                                                                                                                                                                                                                                                                                       |
| **4** | **Non-directional, non-statistical**                   | a non-directional relationship between two variables is explored in a non-statistical manner, e.g., contingency tables, mosaic plots, stacked bar charts, overlaying two spatial variables on the same map, or qualitative co-occurrence.                                                                                                                                                                                                                                                                                                                            |
| **5** | **Directional, non-statistical**                       | a directional relationship, in which a relating variable influences a target variable, is stated without use of inferential statistics, e.g., claims of influence are supported by evidence such as 1. relative change in a percentage over time, 2. time series of trend reporting, 3. differences of proportions across a set of categories, or narrative causal statements involving evidence from interviews or other qualitative data suggesting that one variable (relating variable) predicts or causes a change in an outcome of interest (target variable); |
| **6** | **Non-directional, statistical, significant**          | a non-directional relationship between two variables is explored using statistics and found to be significant, e.g., Pearsons's r (correlation between normally distributed, continuous variables), Spearman's rank correlation (correlation between variables that are non-normally distributed), Chi-squared (used for categorical variables), and log-linear analysis (used to explore relationship between three or more categorical variables);                                                                                                                 |
| **7** | **Non-directional, statistical, not significant**      | a non-directional relationship between two variables is explored using statistics and found NOT to be significant;                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **8** | **Non-directional, statistical, unknown significance** | a non-directional relationship between two variables is not reported or undetermined, i.e., no statistical results were reported by the authors;                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **9** | **Relationship exists but type is unknown**            | it is not possible to identify whether the relationship was directional or non-directional, statistical or non-statistical, but it is clear that the author assumes a relationship between two variables.                                                                                                                                                                                                                                                                                                                                                            |

### **14.3.3 Relationship Identification Goal**

For every indicator, the AI **must identify its role in predictive
relationships (X-\>Y) where the link is not already defined by the
constitutive sub-variable calculation**, as directed in section [14.3.1
X-Y Relationship Exclusion and Inclusion
Rules](#1431-x-y-relationship-exclusion-and-inclusion-rules). The
following elements must be identified:

| Relationship Element      | Definition/Context                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:-----------------------------------|:-----------------------------------|
| **Relating Variable (X)** | Determine which indicators serve as the predictor (X) for other indicators (Y) in the study. A relating variable is any indicator (X) that is used to explore its relationships to another indicator (Y), and may include indicators characterized as a directly measured continuous/count, ordinal, nominal, or narrative variable, or any type of outcome variable. A special type of relating variable is a **narrative causal element** which is the relating variable (X) in a **narrative causal statement**.     |
| **Target Variable (Y)**   | Determine which indicators serve as the outcome (Y) being influenced by other indicators (X) in the study. A target variable is any indicator (Y) for which relationships with other indicators (X) are explored, and may include indicators characterized as a directly measured continuous/count, ordinal, nominal, or narrative variable, or any type of outcome variable. A special type of target variable is a **narrative causal outcome** which is the target variable (Y) in a **narrative causal statement**. |
| **Relationship Type**     | Determine the numerical code (Type 1 through 9) from the X-Y typology in section [14.3.2 X-Y Relationships to Record](#1432-x-y-relationships-to-record) for each identified relationship.                                                                                                                                                                                                                                                                                                                              |

### **14.3.4 Predictive Symmetry Rule (Cross-Referencing Output)**

When populating the output table columns for X-Y relationships, the AI
must ensure complete symmetrical cross-referencing using the following
rules:

| Indicator Role                         | Target Variable Column (X's Row)                                      | Relating Variable Column (Y's Row)                                                                                             | Notes                                                                                         |
|:-----------------|:-----------------|:-----------------|:-----------------|
| **Relating Variable (X)**              | Must list indicator number(s) of its Target variable(s) (Y).          | Must list **n/a**.                                                                                                             | Designates which variable is the predictor.                                                   |
| **Target Variable (Y)**                | Must list **n/a**.                                                    | Must list indicator number(s) of reciprocal Relating variable(s) (X) + **(Type Code)**, separated by semi-colons (e.g., 4(5)). | Ensures symmetrical cross-referencing and includes the relationship type.                     |
| **Non-Directional (Types 4, 6, 7, 8)** | Arbitrarily assign one as X and one as Y. The X row lists Y's number. | The Y row lists X's number + (Type Code).                                                                                      | Relationship is recorded only once across the entire table using the single X-\>Y assignment. |

### **14.3.5 Principle of Systemic Causality**

When coding relationships in a complex model (like a bioeconomic
simulation), the X-Y relationship typology (Type 1 through 9) must be
reserved only for **emergent, high-level causal pathways and feedback
loops** that define the system's management hypotheses or aggregate
effects. This focuses analysis on the system-level interactions that
mirror traditional predictive or causal analysis (e.g., policy levers
and demographic feedback loops).

# **15.0 Asked/stated vs Measured/observed (Data Source 3)**

The following typology should be used to select the best code for the
**Asked/stated vs Measured/observed (Data Source 3)** of the indicator:

|  Code   | Asked/stated vs Measured/observed (Data Source 3) Type | Definition                                                                                                                                                                                                                                                                       | Special Instructions                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|:-----------------:|:-----------------|:-----------------|:-----------------|
|  **1**  | **Asked/stated**                                       | The information used to assess/score this indicator was derived through direct interaction with human subjects (e.g., asking people about to state their preferences or for them to report personal or localized knowledge of fish stocks or sales, etc.).                       | 1\. **Special Instruction 1 (Secondary Data)**: If the indicator is assessed/scored based on secondary data (i.e., **Primary vs Secondary** is coded as Secondary based on the typology in section [10.0 Primary vs Secondary (Data Source 2)](100-primary-vs-secondary-data-source-2), then determination of the Asked/stated vs Measured/observed (Data Source 3) code **must consider whether the original data collection involved interaction with human subjects**; 2. **Special Instruction 2 (Outcome Types 6, 7, 8, and 11)**: If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Asked/stated** (Code 1) **ONLY if** both the following conditions are met: a. all associated sub-variables received Code 1 in the Asked/stated vs Measured/observed column, and b. no associated sub-variables were modeled (Code 2 in the Empirical vs Modeled column). |
|  **2**  | **Measured/observed**                                  | The information used to assess/score this indicator was derived through direct observation or measurement (e.g., participant observation with fieldnotes, or biological/ecological measurements, etc.).                                                                          | 1\. **Special Instruction 1 (Secondary Data)**: If the indicator is assessed/scored based on secondary data (i.e., **Primary vs Secondary** is coded as Secondary based on the typology in section [10.0 Primary vs Secondary (Data Source 2)](100-primary-vs-secondary-data-source-2), then determination of the Data Source 3 code **must consider whether the original data collection involved direct measurement or observation by researchers**; 2. **Special Instruction 2 (Outcome Types 6, 7, 8, and 11)**: If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Measured/observed** (Code 2) **ONLY if** both of the following conditions are med: a. all associated sub-variables received Code 2 in the Asked/stated vs Measured/observed column and b. no associated sub-variables were modeled (Code 2 in the Empirical vs Modeled column).             |
|  **3**  | **Statistically derived**                              | The indicator's assessed value is the product or output of a complex mathematical or statistical simulation, including dynamic system models (e.g., bio-economic, ecosystem dynamics, forecasting).                                                                              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|  **4**  | **Undetermined**                                       | Information is reported about the data source of the indicator, but the distinction of the data source as either involving interaction with human subjects, involving direct measurements and observations, or being statistically derived values cannot be clearly established. | If the indicator is an outcome variable coded as **outcome type** 6, 7, 8, or 11, AI must code the indicator as **Undetermined** (Code 4) if either of the following conditions is met: a. associated sub-variables received a combination of codes 1 and 2 in the column Asked/stated vs. Measured/observed, or b. at least one associated sub-variable received the entry "undetermined" (Code 4) or "n/r" in the Asked/stated vs Measured/observed column.                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **n/r** | **Not reported**                                       | No information is reported in the source text regarding whether the assessed values of the indicator were derived from interaction with human subjects, direct measurements or observations, or are statistically derived.                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

## **15.1 Special Rules for Asked/stated vs Measured/observed (Data Source 3)**

### **Rule 15.1.1 Data Source 3 Symmetry Rule (Statistically Derived)**:

If the **Empirical vs Modeled (Data Source 1)** column in section [9.0
Empirical vs Modeled (Data Source
1](#90-empirical-vs-modeled-data-source-1) for this indicator is coded
as Modelled (Code 2), this Data Source 3 column must be symmetrically
coded as Statistically derived (Code 3).

### **Rule 15.1.2 Empirical Constraint**:

If the **Data Source 1** column in section [9.0 Data Source 1 Empirical
vs Modeled)(#90-data-source-1-empirical-vs-modeled) for this indicator
is coded as **Empirical (Code 1)**, the **Data Source 3** column **must
be coded as either Asked/stated (Code 1) or Measured/observed (Code
2).** It cannot be coded as Statistically derived (Code 3).

## **15.2 Examples of Coding for Asked/stated vs Measured/observed (Data Source 3)**

| Example                                                                                                                                                                      | Asked/stated vs Measured/observed (Data Source 3) Type | Correct Data Source 3 Code |
|--------------------|--------------------|:------------------------------:|
| Researchers carry out primary data collection interviews with fishers regarding information contained in fishers' logbooks                                                   | Asked/stated                                           |             1              |
| Researchers rely on secondary information from a previous study which reported results from interviews with fishers regarding information contained in the fishers' logbooks | Asked/stated                                           |             1              |
| Researchers review fisher logbooks directly (secondary data), and know that the logbook data represent direct observations and measurements recorded by the fishers          | Measured/observed                                      |             2              |
| Researchers carry out participant observation and make field notes that they then use as a basis for indicators                                                              | Measured/observed                                      |             2              |
| Researchers ask sellers at a fish market about how their prices have changed between last year and this year                                                                 | Asked/stated                                           |             1              |
| Changes in real-time market prices written down by a researcher to create a record of real-time price fluctuations                                                           | Measured/observed                                      |             2              |
| Latent classes derived through latent class analysis                                                                                                                         | Statistically derived                                  |             3              |

# **16.0 Instructions for Producing Tables of Indicators and their Attributes**

## **16.1 Rules for All Tables**

**Validation Rule**: Before presenting any final table output
(spreadsheet format), the AI must perform a **Self-Correction Validation
Pass** to confirm cell and column integrity. Specific elements of this
self-correction validation pass are detailed in sections 16.1.1 through
16.1.4.

### **16.1.1 Mandatory Pipe Check (Structural Integrity)**:

Verify that every row contains the exact, correct number of column
separators (pipe symbols, \|), ensuring there are no missing or extra
separators that would cause cell data to merge or shift columns when
transferred to a spreadsheet.

### **16.1.2 Special Entry Check (Multi-word Robustness)**:

Pay particular attention to cells containing multi-word entries, such as
"see sub-variables," "Other derived outcome," and long text strings, to
ensure the pipe separation remains robust on both sides.

### **16.1.3 Data Alignment Confirmation (Positional Check)**:

Confirm that the value in the Associated Outcome Variable column and the
value in the Unit of Analysis column are correctly separated and not
shifted left.

### **16.1.4 Blank Column Placeholder Mandate (Qualitative Stability)**:

For all columns designed to contain qualitative feedback, rationale, or
textual notes (e.g., the 'Conceptual Distinction Issues' and 'Suggested
Definition Edits' columns in Tables 3, 4, and 5, or the 'Relationship
Rationale' column in Table 2), the AI must not leave the cell blank if
no relevant information is found or if the GIP mandates that a
particular attribute is not applicable. In such cases, the AI must
populate the cell with the placeholder **"n/a"** (not applicable/no
entry) to prevent column drift and confirm the AI has assessed the cell.

## **16.2 Table 1 specifications**

Based on a research article I upload, I would like the AI to create a
table that lists each of the indicators identified within the text,
figures, and/or tables in the article, based on the rules for inclusion
of a variable as a unique indicator outlined in the section [2.0
Instructions for Identifying Relevant
Indicators](#20-instructions-for-identifying-relevant-indicators) and
following the **validation rule** in section [16.1 Rules for All
Tables](#161-rules-for-all-tables) and the **categorical label exclusion
constraint** in section [16.2.1 Rules for Table
1](#1621-rules-for-table-1).

### **16.2.1 Rules for Table 1**

#### **16.2.1.1 Mandatory Consolidation for Simple Nominal Labels (The Nominal Label Constraint)**:

The AI **must consolidate** multiple entries that represent the
**mutually exclusive states, labels, or indices of a single nominal or
categorical variable** if these states share the exact same Name of
Indicator, Definition of Indicator, **AND** lack distinct Variable
Assessment Details. This rule prevents redundant listing of category
labels (e.g., Policy Scenario 'A', 'B', 'C') for a high-level
categorical variable (e.g., 'Policy Scenario Type').

#### **16.2.1.2 Measurement Component Inclusion Mandate**:

Notwithstanding the constraint in section [16.2.1.1 Mandatory
Consolidation for Simple Nominal Labels (The Nominal Label
Constraint](#16211-manadatory-consolidation-for-simple-nominal-labels-the-nominal-label-constraint),
the AI **MUST NOT consolidate** or exclude any variable that represents
a granular **Variable Assessment Detail (VAD)** if that VAD is necessary
for either: (a) Measuring a single conceptual variable (e.g., an
individual Likert Question), or (b) Acting as a constitutive input to a
higher-level Composite Index (Code 6) or Latent Construct (Code 7).

### **16.2.2 Table 1 Column Specifications**

The AI **must number each row** in Table 1 and **must choose an
indicator title that aligns with how the indicator has been presented in
the research article.** Following the column with the indicator name,
**the following attributes must each be included in their own column**:

```         
1. **Inclusion Justification**: In this column, identify the sole criterion by which the indicator qualified for inclusion in the list. Use the following three categories, which relate to the rules outlined in the "Instructions for Identifying Relevant Indicators" section:
```

| Code  | Criterion                | Full Definition                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|:--------------------------:|:---------------------|:---------------------|
| **1** | **Named/Defined**        | The indicator met the inclusion criteria because its name or definition was explicitly provided by the authors. This applies to most conventionally described indicators.                                                                                                                                                                                                                                                                                                                                                                                        |
| **2** | **Score Only**           | The indicator met the inclusion criteria solely because a numerical value was reported for it, overriding the need for an explicit name or definition.                                                                                                                                                                                                                                                                                                                                                                                                           |
| **3** | **Inferred (SADP)**      | The indicator was included notwithstanding the 'separately detailed' criterion described in section [2.0 Instructions for Identifying Relevant Indicators](#20-instructions-for-identifying-relevant-indicators) because it was required to complete an aggregate mathematical linkage (A -\> X -\> C) necessary to satisfy the Standard Aggregate Decomposition Protocol (SADP) described in section [14.2.1 Preparatory Mandates (Defining the Data Set)](#1421-preparatory-mandates-defining-the-data-set). This applies only to inferred intermediate nodes. |
| **4** | **Inferred (Narrative)** | The indicator was explicitly included because it is an essential component (either the Narrative Causal Element (X) or the Narrative Causal Outcome (Y)) of a Narrative Causal Statement (NCS) found in the source text, as mandated by Rule 2.1.4. This inclusion overrides the 'separately detailed' criterion and is applied when the variable is inferred from primary qualitative data synthesis but lacks explicit naming, definition, or a quantitative score.                                                                                            |

```         
2. **Pre-scoring variable type**: If this indicator involves a variable that was directly assessed, and the variable type upon scoring reflects a transformation of original raw data, the variable type of the original, raw data can be reported here in this column using the **basic variable types** outlined in the section [3.0 Variable Type Typology](#30-variable-type-typology). If no transformation is reported, write "n/r."

* **Inclusion Constraint**: If the indicator's **Outcome type** is any form of calculated outcome (Composite index, Latent construct, Other derived outcome), a Model output, or a Categorical outcome, this column **must state "see sub-variables."**

3. **Variable type upon scoring**: If this indicator involves a variable that was directly assessed, record in this column the **basic variable type** that best characterizes the variable at the time of scoring/assessment, using the basic variable type Codes 1-4 described in section [3.0 Variable Type Typology](#30-variable-type-typology), or write "n/r" if no information is reported about variable type upon scoring.
```

-   **Modeling Input Exception**: If the indicator is used as baseline
    data or a model input (as described in the Note on Input Parameters
    in Section 3.3) and this input itself is a pre-calculated aggregate
    from another study or source, record the corresponding outcome type
    code (5, 6, 7, 8, 10, or 11) here. If applicable, amend the code
    with "n" or "o" to indicate nominal or ordinal type (e.g., "5n").

    -   **Inclusion Constraint**: If the indicator's **Outcome type** is
        any form of calculated outcome (Composite index, Latent
        construct, Other derived outcome), a Model output, or a
        Categorical outcome, this column **must state "see
        sub-variables."**

    4.  **Outcome type**: If this indicator involves a calculated
        outcome (Code 6, Code 7, or Code 8), a categorical outcome (Code
        11) or a model output (Code 10), record the outcome type code in
            this column, using the outcome types outlined in the section
            [3.0 Variable Type Typology](#30-variable-type-typology). If
            this indicator involves a variable that was directly
            assessed, write "n/r" in this column unless a descriptive
            statistic summarizing the variable scores is provided, in
            which case record the code 5.
    5.  **Variable type of outcome**: If a code is recorded in the
        **Outcome Type** column, record the variable type of the outcome
        variable or descriptive statistic in this column, using the
        basic variable type codes outlined in the section [3.1 Basic
        Variable Types (Direct Measurement
        Attributes)](#31-basic-variable-types-direct-measurement-attributes).
        If "n/r" was reported in the **Outcome Type** column, the entry
        in this column should also be "n/r."

## **16.3 Table 2 specifications**

Using the same list of indicators generated in Table 1, the AI must
populate Table 2 with a set of attributes of the indicator list across a
series of columns. Creation of Table 2 must follow the **Validation
Rule** in section [16.1 Rules for All Tables](#161-rules-for-all-tables)
and the rules outlined in [16.3.1 Rules for Table
2](#1631-rules-for-table-2).

### **16.3.1 Rules for Table 2**

## **Global Constraint for Non-Directional Relationships (Types 4, 6, 7, 8, and 9)**:

For non-directional relationships, the entire relationship link must be
recorded only once across the entire table. The AI must arbitrarily
assign one variable as the Relating variable (X) and the other as the
Target variable (Y). The remaining variable columns (Target and
Relating) must be populated exclusively following the single X-\>Y
assignment and the column definitions above provided in the
specifications for this table in section [16.3.2 Table 2 Column
Specifications](#1632-table-2-column-specifications).

**Example of Non-Directional Coding (Variable A assigned X, Variable B
assigned Y)**:

-   **Row A (X)**: Target variable column lists [Number of B]. Relating
    variable column lists n/a.

-   **Row B (Y)**: Target variable column lists n/a. Relating variable
    column lists [Number of A].

**Predictive Symmetry Rule**: When populating the output table columns
for X-Y relationships, the AI must ensure complete symmetrical
cross-referencing using the following rules:

-   **Target Variable Column (X's Row Only)**: If the indicator is the
    Relating variable (X), this column must list the indicator number(s)
    of its Target variable(s) (Y).

-   **Relating Variable Column (Y's Row Only)**: If the indicator is the
    Target variable (Y), this column must list the indicator number(s)
    of its reciprocal Relating variable(s) (X). For each relating
    variable listed, the corresponding X-Y relationship type code (1
    through 9) as defined in section [14.3.2 X-Y Relationships to
    Record](#1432-x-y-relationships-to-record), must be appended in
    parentheses for each identified relationship, separated by
    semi-colons (e.g., If predictors #2 and #5 both influence the
    current indicator, the entry might look like: 2(5); 5(1)).

-   **Enforced Exclusivity**: The assigned Y variable must list n/a in
    its Target variable column, and the assigned X variable must list
    n/a in its Relating variable column.

\*\* Code Reference Validation Check\*\*: When populating the Relating
variable column in Table 2, the AI must ensure that:

-   **Symmetry Check**: The indicator number preceding the parentheses
    (the Reciprocal Relating Variable, X) must correspond to a row where
    the Target variable column lists the current indicator's number.

-   **X-Y Relationship Type Codes**: The code inside the parentheses
    (the X-Y Relationship Type) must be drawn exclusively from the list
    of X-Y Relationship Type Codes (1 through 9) detailed in section
    [14.3.2 X-Y Relationships to
    Record](#1432-x-y-relationships-to-record).

-   **Cross-Typology Check**: The code inside the parentheses must not
    be any of the codes reserved for Outcome Variable Types (6, 7, 8,
    10, or 11), preventing the accidental use of the Outcome Type as the
    Relationship Type.

### **16.3.2 Table 2 Column Specifications**

The AI must use the same indicator order and numbering for Table 2 as
was included in the final Table 1 output. Following the column with the
indicator name, **the following attributes must each be included in
their own column**:

```         
1. **Associated Outcome Variable**: If this indicator is a **sub-variable** used to calculate an **Associated Outcome Variable**, list the number(s) of the associated outcome variables in this column. The AI must only report an indicator as an Associated Outcome Variable if the current indicator is an immediate, constitutive sub-variable—meaning the current indicator's value is a necessary input (a term, factor, or argument) in the mathematical calculation of that Outcome Variable's value. **This must strictly follow the Immediate Constitutive Link Rule (One-Step Constitutive Rule)** described in section [14.2.2 Immediate Constitutive Link Rule (Defining the Structural Requirements)](#1422-immediate-constitutive-link-rule-defining-the-structural-requirements): **it must not list any outcome variable calculated from the immediate associated outcome (X -> Y -> Z is forbidden).** If this indicator is not a sub-variable used to calculate an associated outcome variable, write “n/a” in this column. For details see the section [14.2 Sub-variables and Outcome Variables.](#142-sub-variables-and-outcome-variables).

2. **Associated Sub-variable**: If this indicator is an **outcome variable** that is calculated using **Associated Sub-variables** listed in the table, list the number(s) of the relevant sub-variables in this column. If this indicator is not an outcome variable calculated from other sub-variables listed in this table, write “n/a” in this column. For further details see section [14.2 Sub-variables and Outcome Variables.](#142-sub-variables-and-outcome-variables).

3. **Target variable**: If this indicator is a **Relating variable (X)**, list the indicator number(s) of the associated **Target variables (Y)** in this column. If this indicator is a Target variable (Y), this column **must be marked with "n/a"** to prevent redundant recording of the relationship link. If this indicator is neither a relating nor a target variable, write "n/a" in this column.

4. **Relating variable**: If this indicator is a **Target variable (Y)**, list the indicator number(s) of the associated **Relating variables (X)**. **For each relating variable listed, the corresponding X-Y relationship type code (1 through 9), as defined in section [14.3.2 X-Y Relationships to Record](#1432-x-y-relationships-to-record), must be appended in parentheses for each identified relationship, separated by semi-colons (e.g., 2(5); 5(1)).** If this indicator is a Relating variable (X), this column **must be marked with "n/a"**.
```

-   **Mandate for X-Y Code Validation**: For every entry in this column
    containing a relationship code (1 through 9), the AI must perform a
    final internal audit to confirm that the assigned code adheres to
    the Mandatory Two-Step X-Y Relationship Verification Protocol
    defined in Section 14.3.2. Specifically, Code 1 (Directional,
    statistical, significant) and Code 6 (Non-directional, statistical,
    significant) must be reserved strictly for relationships where the
    statistical analysis reported $p < 0.05$ (or equivalent metric).
    Codes 2 and 7 must be used for non-significant statistical findings.

    5.  **Relationship Rationale**: The AI **must** provide a concise,
        cross-referenced rationale in this dedicated final column of
        Table 2, explaining the indicator's complete structural and
        predictive role. The rationale must address two components:

A. **Constitutive Role (Sub-variable / Outcome Variable)**: Explain the
immediate calculation role (Input to Y or Output from X). B.
**Predictive Role (Relating / Target Variable)**: For any link recorded
in the **Target variable** or **Relating variable** columns, explain the
assignment based on the GIP's X-Y Relationship Exclusion/Inclusion Rules
(Section 14.3.1). The rationale **must explicitly categorize the link's
predictive basis**, stating whether the link's inclusion in the
predictive columns is based on the structural relationship or an
entirely separate causal test: \> \* **Structural-Only Role /
Definitional Identity (Rule 1)**: Link is Constitutive, and **Excluded
from predictive X-Y analysis** because it is a Mathematical Identity or
Accounting Aggregation. (Link is Constitutive-Only). \> \*
**Causal-Testing Role / Statistical Causal Estimate (Rule 3)**: Link is
Constitutive, and **Included in predictive X-Y analysis** because the
**structural relationship itself** was actively tested or quantified for
a causal influence (e.g., parameter estimation, coefficient
calculation). The rationale **MUST** explicitly state that the same
structural link is being used for both **Architectural Mapping**
(Constitutive) and **Hypothesis Testing** (Predictive), and be
classified as: (Link is **Constitutive/Predictive**). \> \*
**Causal-Testing Role / External Causal Role (Rule 2)**: Link is
**Included in predictive X-Y analysis** because the indicator was used
as a predictor in a **separate, non-constitutive X-Y analysis** (e.g.,
an input is correlated with the final high-level outcome, not its
immediate calculation). (Link is Predictive-Only).

**Clarification Mandate:** For indicators satisfying Rule 3, the
rationale must explicitly state that the same structural link is being
used for both **Architectural Mapping** (Constitutive) and **Hypothesis
Testing** (Predictive).

-   **Format Constraint**: The relationship rationale should be brief,
    clearly identifying the structural relationship and its
    classification (e.g., "Constitutive: Direct calculation for Fst (Eq.
    1). Predictive: **Constitutive/Predictive (Rule 3)**, structural
    link tested/calibrated for causal influence.").

## **16.4 Table 3 specifications**

Using the same list of indicators generated in Table 1, the AI must
populate Table 3 with a set of attributes of the indicator list across a
series of columns. Creation of Table 3 must follow the **Validation
Rule** in section [16.1 Rules for All
Tables](#161-rules-for-all-tables).

### **16.4.1 Table 3 column specifications**

The AI must use the same indicator order and numbering for Table 3 as
was included in the final Table 1 output. Following the column with the
indicator name, **the following attributes must each be included in
their own column**:

1.  **Sub-category of Primary Variable Concept**: Identify the **primary
    variable concept** following the definitions and procedures in
    section [14.0 Relationships Within and Between
    Indicators](#140-relationships-within-and-between-indicators). Then,
    using the primary category definitions and sub-category definitions
    provided in section [13.0 Conceptual
    categories](#130-conceptual-categories), locate the sub-category
    definition that best captures the **primary conceptual assessment
    target** (the **primary variable concept**). The conceptual
    sub-category matching process **must strictly follow the steps and
    rules** laid out in section [13.1 Process for matching a concept to
    a
    sub-category](#131-process-for-matching-a-concept-to-a-sub-category).

    -   **Format Constraint (Naming)**: Write the exact wording of the
        selected sub-category name (e.g., "Condition of fish stocks").

    -   **Inclusion Rule (Focus on Assessment Target)**:

        a.  Rule A (Direct or Calculated Target): If the indicator is a
            direct measurement (Basic Variable Type) OR if the indicator
            is a Calculated Outcome (Codes 6, 7, 8, 10), the Primary
            Variable Concept must be the concept of the final assessed
            or calculated output.
        b.  Rule B (Conceptual or Sub-variable Focus): If the indicator
            is a Constitutive Sub-variable (Role 3, 4, or 5 in Table 4)
            OR if the indicator is a Categorical Outcome (Code 11), this
            column must state "see sub-variables."

2.  **Definition Match for Primary Variable Concept**: In this column,
    the AI **must list specific words or phrases** that led the AI to
    match the **primary variable concept** to the selected sub-category
    definition.

    -   **Definition Validation Format Constraints**: If the **primary
        variable concept** the AI is matching to the sub-category is
        already reflected in the existing sub-category definition, the
        AI **must include the exact words and phrases from the
        definition that match the concept.** If the primary variable
        concept the AI is locating in the sub-category **is not
        explicitly referenced in the existing sub-category definition,
        the AI must suggest adjustments or additions to the sub-category
        definition** in brackets, e.g., "[I suggest adding "social
        capital" to this definition]".
    -   **Inclusion Constraint**: If the indicator's **Outcome type** is
        any form of calculated outcome (Composite index, Latent
        construct, Other derived outcome), a Model output, or a
        Categorical outcome, this column **must state "see
        sub-variables."**

3.  **Sub-categor(ies) of Secondary Variable Concept(s)**: Identify any
    **secondary variable concepts** following the definitions and
    procedures in section [14.0 Relationships Within and Between
    Indicators](#140-relationships-within-and-between-indicators). Then,
    using the primary category definitions and sub-category definitions
    provided in section [13.0 Conceptual
    categories](#130-conceptual-categories), locate the sub-category
    definition that best matches the secondary variable concept. The
    conceptual sub-category matching process **must strictly follow the
    steps and rules** laid out in section [13.1 Process for matching a
    concept to a
    sub-category](#131-process-for-matching-a-concept-to-a-sub-category).

    -   **Mandate for Calculated Outcomes (Codes 6, 7, 8, 10)**: If the
        indicator is a Calculated Outcome, the AI **must** apply
        **Protocol 14.1.2.7 (Equation Secondary Variable Concept)** and
        list the conceptual sub-category of every implicit or explicit
        component used in the indicator's calculation/formula that is
        not already listed as an **Associated Sub-variable** in Table 2.
    -   **Format Constraint (Naming)**: Write the exact wording of the
        selected sub-category name (e.g., "Condition of fish stocks").
    -   **Format Constraint (Multiplicity)**: If multiple secondary
        conceptual elements are reported, the conceptual sub-categories
        for each element **must be separated by a semi-colon (;).**
    -   **Inclusion Constraint**: If the indicator's **Outcome type** is
        any form of calculated outcome (Composite index, Latent
        construct, Other derived outcome), a Model output, or a
        Categorical outcome, this column **must state "see
        sub-variables."**

4.  **Definition Match for Secondary Variable Concept(s)**: In this
    column, the AI **must list specific words or phrases** that led the
    AI to match the **secondary variable concept** to the selected
    sub-category definition.

    -   **Definition Validation Format Constraints**: If the **secondary
        variable concept** the AI is matching to the sub-category is
        already reflected in the existing sub-category definition, the
        AI **must include the exact words and phrases from the
        definition that match the concept.** If the secondary variable
        concept the AI is matching to the sub-category **is not
        explicitly referenced in the existing sub-category definition,
        the AI must suggest adjustments or additions to the sub-category
        definition** in brackets, e.g., "[I suggest adding "social
        capital" to this definition]".

-   **Format Constraint (Multiplicity)**: If multiple definition matches
    are reported, the description for each element must be separated by
    a semi-colon (;).

5.  **Sub-category of Indicator topic**: Identify the **indicator
    topic** following the definitions and procedures in section [14.0
    Relationships Within and Between
    Indicators](#140-relationships-within-and-between-indicators). Using
    the primary category definitions and sub-category definitions
    provided in section [13.0 Conceptual
    categories](#130-conceptual-categories), locate the sub-category
    definition that best captures the indicator's **conceptual
    representation target** (the **indicator topic**). The conceptual
    sub-category matching process **must strictly follow the steps and
    rules** laid out in section [13.1 Process for matching a concept to
    a
    sub-category](#131-process-for-matching-a-concept-to-a-sub-category).

    -   **Format Constraint (Naming)**: Write the exact wording of the
        selected sub-category name (e.g., "Condition of fish stocks").

6.  **Definition Match for Indicator Topic**: In this column, the AI
    **must list specific words or phrases** that led the AI to match the
    **indicator topic** to the selected sub-category definition.

    -   **Definition Validation and Feedback**: If the concept the AI is
        locating in the sub-category is already reflected in the
        existing sub-category definition, the AI **must include the
        exact words and phrases from the definition that match the
        concept.** If the concept the AI is locating in the sub-category
        is not explicitly referenced in the existing sub-category
        definition, the AI **must suggest adjustments or additions to
        the sub-category definition** in brackets, e.g., [I suggest
        adding "social capital" to this definition].

## **16.5 Table 4 specifications**

Using the same list of indicators generated in Table 1, the AI must
populate Table 4 with a set of attributes of the indicator list across a
series of columns. Creation of Table 4 must follow the **Validation
Rule** in section [16.1 Rules for All
Tables](#161-rules-for-all-tables).

### **16.5.1 Table 4 column specifications**

The AI must use the same indicator order and numbering for Table 4 as
was included in the final Table 1 output. Following the column with the
indicator name, **the following attributes must each be included in
their own column**:

1.  **Alternative Sub-category Matches**: In this column, the AI **must
    list all sub-categories** that were identified as possible in Table
    3, but not ultimately chosen, matches for the concepts being
    evaluated (Primary Variable Concept, Secondary Variable Concept(s),
    and Indicator Topic).

| Output Instruction | Detail                                                                     |
|:--------------------------------------:|:-------------------------------|
| **Data Required:** | List the exact sub-category names for all plausible alternative matches.   |
| **Input Source:)** | Generated during the conceptual matching process detailed in Section 13.1. |

-   **Format Constraint (Entry Separation)**: Entries for each concept
    being reviewed (e.g., Primary Concept vs. Indicator Topic) must be
    separated by a double pipe ("\|\|") for each distinct entry.
-   **Format Constraint (Internal Delimiter)**: Within an entry,
    alternative sub-category names **must be separated by a semi-colon
    (;)** for each distinct sub-category (e.g., Alternative A;
    Alternative B).
-   **Format Constraint (Internal Labeling)**: Each entry **must be
    prefixed with a label identifying the conceptual element being
    reviewed,** as defined in the table below:

|       Internal Label        | Concept Type Evaluated                               | Example Format                                      |
|:--------------------------:|:---------------------|:---------------------|
|    **Primary Concept:**     | The core assessed variable.                          | **Primary Concept:** *Alternative A; Alternative B* |
| **Secondary (Specifying):** | The specific detail component (Code 14.1.2.6).       | **Secondary (Specifying):** *Alternative C*         |
|  **Secondary (Equation):**  | The implicit calculation component (Code 14.1.2.7).  | **Secondary (Equation):** *Alternative D*           |
| **Secondary (Predictor):**  | The internal hypothesized influence (Code 14.1.2.8). | **Secondary (Predictor):** *Alternative E*          |
|    **Indicator Topic:**     | The overall conceptual goal of the indicator.        | **Indicator Topic:** *Alternative F; Alternative G* |

2.  **Conceptual Distinction Issues**: This column captures the
    qualitative feedback regarding any perceived lack of clarity,
    ambiguity, or conceptual overlap between definitions in the GIP's
    conceptual framework outlined in section [13.0 Conceptual
    categories](#130-conceptual-categories) (Section 13.0) encountered
    while attempting to code the Primary, Secondary, or Topic concepts.

|         Output Instruction         | Detail                                                                                                                                                                                                                   |
|:--------------------------------------:|:-------------------------------|
| **Conceptual Distinction Issues:** | Describe the ambiguity encountered. This includes issues like insufficient detail in a definition, logical inconsistency, or a conceptual overlap that makes the distinction between two or more sub-categories unclear. |
|         **Input Source:)**         | Generated during the conceptual matching process detailed in Section 13.1.                                                                                                                                               |

-   **Format Constraint (Entry Separation)**: Entries for each concept
    being reviewed (e.g., Primary Concept vs. Indicator Topic) **must be
    separated by a double pipe (\|\|)** for each distinct entry.
-   **Format Constraint (Internal Labeling)**: Each entry **must be
    prefixed with a label identifying the conceptual element being
    reviewed,** as defined in the table below:

|       Internal Label        | Concept Type Evaluated                               | Example Format                                                                                              |
|:--------------------------:|:---------------------|:---------------------|
|    **Primary Concept:**     | The core assessed variable.                          | **Primary Concept:** Need clarity on whether social services include housing or are just focused on health. |
| **Secondary (Specifying):** | The specific detail component (Code 14.1.2.6).       | **Secondary (Specifying):** he boundaries between engagement and political capital are too vague here.      |
|  **Secondary (Equation):**  | The implicit calculation component (Code 14.1.2.7).  | **Secondary (Equation):** Definition 8 needs to state if it covers complex ratios or only simple sums.      |
| **Secondary (Predictor):**  | The internal hypothesized influence (Code 14.1.2.8). | **Secondary (Predictor):** Is fishing pressure always environmental, or can it be an economic output?       |
|    **Indicator Topic:**     | The overall conceptual goal of the indicator.        | **Indicator Topic:** Vague boundary between social and ethical sustainability.                              |

3.  **Suggested Definition Edits**: This column captures the actionable
    advice derived from the AI's conceptual matching experience,
    providing specific text modifications intended to resolve
    ambiguities or overlaps in the GIP's existing typology (Section
    13.0).

|             Content             | Instruction                                                                                                                                           |
|:--------------------------------------:|:-------------------------------|
| **Suggested Definition Edits:** | Provide the specific text that should be added to or removed from the relevant sub-category definition to clarify boundaries or add missing concepts. |

-   **Format Constraint (Entry Separation)**: Entries for each concept
    being reviewed (Primary, Secondary, or Topic) **must be separated by
    a double pipe ("\|\|")** for each distinct entry.
-   **Format Constraint (Internal Labeling)**: Each entry **must be
    prefixed with a label identifying the conceptual element being
    reviewed, followed by a colon and a space "(: )".**
-   **Format Constraint (Actionable Text)**: All suggested additions,
    removals, or adjustments to the typology text **must be enclosed in
    square brackets "[]"** to clearly delineate the recommended change
    from the descriptive text, as defined in the table below:

|       Internal Label        | Concept Type Evaluated                               | Example Format                                                                                                           |
|:--------------------------:|:---------------------|:---------------------|
|    **Primary Concept:**     | The core assessed variable.                          | **Primary Concept:** [Recommend adding "self-esteem" to the definition of Emotional capital]                             |
| **Secondary (Specifying):** | The specific detail component (Code 14.1.2.6).       | **Secondary (Specifying):** [Suggest removing the NOTE about political causes from Democratic engagement]                |
|  **Secondary (Equation):**  | The implicit calculation component (Code 14.1.2.7).  | **Secondary (Equation):** [Clarify that 'Other derived outcome' explicitly includes complex ratios]                      |
| **Secondary (Predictor):**  | The internal hypothesized influence (Code 14.1.2.8). | **Secondary (Predictor):** [Add distinction between "Fishing pressure" as an economic input and an environmental output] |
|    **Indicator Topic:**     | The overall conceptual goal of the indicator.        | **Indicator Topic:** [Suggest creating a new sub-category for "Ecosystem Justice" under Ethical sustainability]          |

## **16.6 Table 5 specifications**

Using the same list of indicators generated in Table 1, the AI must
populate Table 5 with a set of attributes of the indicator list across a
series of columns. Creation of Table 5 must follow the **Validation
Rule** in section [16.1 Rules for All
Tables](#161-rules-for-all-tables).

### **16.6.1 Table 5 column specifications**

The AI must use the same indicator order and numbering for Table 5 as
was included in the final Table 1 output. Following the column with the
indicator name, **the following attributes must each be included in
their own column**:

1.  **Conceptual Proxy Present**: If the **primary variable concept**
    and **indicator topic** identified in Table 3 for this indicator are
    located in distinct conceptual sub-categories, the AI must indicate
    in this column that a conceptual proxy is present for the indicator.

    -   **Inclusion Constraint (Derived Indicators)**: If the
        indicator's **Outcome type** (Table 1) is any form of calculated
        outcome (Composite index (6), Latent construct (7), Other
        derived outcome (8)), a Model output (10), or a Categorical
        outcome (11), this column **must state "see sub-variables."**

2.  **Management purpose theme**: Select the most accurate management
    purpose that this indicator is used to support from the list of
    management purpose themes provided in the section [11.0 Management
    Purpose Themes](#110-management-purpose-themes).

    -   **Format Constraint**: Write the exact wording of the term of
        the selected management purpose theme (e.g., "Ambient
        monitoring").

3.  **Rationale for Management Purpose Theme Code**: A brief explanation
    justifying the selection of the Management Purpose Theme based on
    the indicator's explicit or implicit use in the study.

4.  **Sustainability theme**: Select the sustainability theme that most
    accurately characterizes the overall framing of the study, using the
    list of sustainability themes provided in the section [12.0
    Sustainability Themes](#120-sustainability-themes).

    -   **Format Constraint**: Write the exact wording of the term of
        the selected sustainability theme (e.g., "Equality, equity, and
        justice").

5.  **Rationale for Sustainability Theme Code**: A brief explanation
    justifying the selection of the Sustainability Theme based on the
    indicator's conceptual fit or the overall framing of the study.

## **16.7 Table 6 specifications**

Using the same list of indicators generated in Table 1, the AI must
populate Table 6 with a set of attributes of the indicator list across a
series of columns. Creation of Table 6 must follow the **Validation
Rule** in section [16.1 Rules for All
Tables](#161-rules-for-all-tables).

### **16.7.1 Table 6 column specifications**

The AI must use the same indicator order and numbering for Table 6 as
was included in the final Table 1 output. Following the column with the
indicator name, **the following attributes must each be included in
their own column**:

1.  **Conceptual relationship code**: As a synthesis of information from
    Table 1, Table 2, Table 3, and Table 5 the AI **must enter the
    code(s) for the conceptual relationship type(s) that best
    characterize this indicator**, following the conceptual relationship
    typology listed in section [4.2 Conceptual Relationship
    Typology](#42-conceptual-relationship-typology). Determining the
    relevant code or codes requires reference to the following elements
    in each of the previous Tables:

    -   **Outcome type**: In Table 1, the **Outcome type** code informs
        whether or not a "6" code is appropriate to include for this
        indicator. Code 6 should be applied if the **outcome type** code
        of the indicator includes a 6, 7, 8, or 11, and/or if the
        indicator lists associated sub-variables in the Associated
        Sub-variable column of Table 2.

    -   **Associated Sub-variable**: In Table 2, whether the indicator
        is identified as an **Associated Sub-variable** and/or as an
        **Associated Outcome Variable** informs whether or not the
        indicator serves as a sub-variable and should be coded as either
        a "3" (Code 3 is correct if an indicator is a sub-variable of a
        **latent construct** outcome type), a "4" (Code 4 is correct if
        an indicator is a sub-variable of a **composite index** outcome
        type), or "5" (Code 5 is correct if an indicator is a
        sub-variable for an **other derived outcome** or a **categorical
        outcome**).

    -   **Presence or Absence of Conceptual Proxy**: In Table 5, the
        presence or absence of a **conceptual proxy**, as described in
        section [14.1.3 Conceptual proxy](#1413-conceptual-proxy)
        informs whether the indicator must be coded as a "2" (Code 2 is
        correct if an indicator contains a within-indicator conceptual
        proxy relationship between the variable concept and indicator
        topic).

    -   **Procedural Hierarchy Check (Codes 1, 2, and 7)**: When
        classifying a standalone (non-constitutive; i.e., Codes 3, 4, 5,
        or 6 are NOT present) indicator that has been separately
        detailed\*\* (i.e., not coded "n/r" in Table 3):Proxy Status
        (Code 2):

        1.  **Proxy Status (Code 2)**: If a Conceptual Proxy is found
            (Primary Variable Concept $\neq$ Indicator Topic in Table
            3), the final classification MUST include Code 2.
        2.  **Direct Measure Status (Code 1)**: If NO Conceptual Proxy
            is found, the classification MUST be Code 1.
        3.  **Descriptive Statistic Override**: The presence of Outcome
            Type Code 5 (Descriptive statistics) DOES NOT preclude the
            application of Code 1 or Code 2.
        4.  **Mutual Exclusivity**: Code 7 (Other) is STRICTLY RESERVED
            for indicators that are $\text{n/r}$ in Table 3 (conceptual
            matching failed due to missing detail) OR act as pure
            macro-level categorical inputs (e.g., non-measurable
            national classifications). Codes 1 and 2 MUST NOT be
            combined with Code 7.

2.  **Rationale for conceptual relationship code**: In this column, the
    AI must describe the reasons why it selected the conceptual
    relationship code or codes for this indicator.

    -   **Format Constraint**: When referencing other indicators, for
        example to explain that the indicator is an outcome variable
        with several associated sub-variables, the number of the
        indicator should be cited rather than the name.

## **16.8 Table 7 Specifications**

Using the same list of indicators generated in Table 1, the AI must
populate Table 7 with a set of attributes of the indicator list across a
series of columns. Creation of Table 7 must follow the **Validation
Rule** in section [16.1 Rules for All
Tables](#161-rules-for-all-tables).

### **16.8.1 Table 7 Special Rules**

-   **Rule 1: Data Source Consistency Check (Empirical/Derived)**: For
    indicators coded Derived in the $\mathbf{Unit \ of \ Observation}$
    column, the corresponding $\mathbf{Data \ Source \ 2}$ and
    $\mathbf{Data \ Source \ 3}$ columns must be populated with Code
    $\mathbf{2}$ (Secondary) or Code $\mathbf{3}$ (Statistically
    derived) to reflect that the data presented were processed or
    aggregated, even if the raw data source was primary.
-   **Rule 2: Scale Exclusion Sync**: Ensure that whenever
    $\mathbf{n/a}$ is present in the $\mathbf{Unit \ of \ Observation}$
    column (for Environmental Context variables, per Rule 6.1.1.3), it
    is symmetrically applied in the $\mathbf{Unit \ of \ Analysis}$
    column (per Rule 7.1.1.1).

### **16.8.2 Table 7 Column Specifications**

The AI **must use the same indicator order and numbering for Table 7 as
was included in the final Table 1 output.** Following the column with
the indicator name, **the following attributes must each be included in
their own column**:

1.  **Community Type**: In this column, if the indicator involves a
    variable that is directly assessed, the AI **must indicate the**
    community type\*\* of the indicator, using the community types
    outlined in the section [5.0 Community Type](#50-community-type). If
    the Outcome Type for this indicator is recorded as a calculated
    outcome (composite index, latent construct, or other derived
    outcome), a model output, or a categorical outcome, the AI must
    determine the Community Type based on the indicator's constitutive
    sub-variables. If sub-variables have differing Community Types, the
    AI should code the most frequently occurring type among the
    immediate inputs.

    -   **Inclusion Constraint**: If both the **variable concept** and
        the **indicator topic** of this indicator were coded to
        sub-categories located within the Environmental Context
        **primary category**, this column **must state "n/a."**

2.  **Unit of Observation**: In this column, if the indicator involves a
    variable that is directly assessed, indicate the unit of observation
    for the variable following instructions in section [6.0 Unit of
    Observation](#60-unit-of-observation). If the indicator is
    identified as one of the Outcome Variable Types included in section
    [3.2 Outcome Variable Types](#32-outcome-variable-types], the AI
    **must record "see sub-variables"** in this column, following the
    constraints outlined in section [6.0 Unit of
    Observation](#60-unit-of-observation).

3.  **Unit of Analysis**: Based on available information in the source
    text regarding **variable assessment details** as defined in section
    [2.0 Instructions for Identifying Relevant
    Indicators](#20-instructions-for-identifying-relevant-indicators),
    as well as the **Outcome Type** and **Variable Type of Outcome** as
    defined in section [3.3 Variable Types at Different Points in
    Time](#33-variable-types-at-different-points-in-time), the AI must
    determine the appropriate Unit of Analysis code (1-6) by checking
    the final presentation of the indicator, following all constraints
    in section [7.0 Unit of Analysis](#70-unit-of-analysis).

4.  **Indicator Action**: In this column, AI must record the most
    accurate code or codes from the Indicator Action code typology
    provided in section [8.0 Indicator Action](#80-indicator-action).
    Indicator Action Code 1 (Evaluation) and Code 2
    (Development/testing) **are not mutually exclusive.**

5.  **Empirical vs Modeled**: In this column, AI must record the most
    accurate code or codes from the Empirical vs Modeled (Data Source 1)
    code typology provided in section [9.0 Empirical vs Modeled (Data
    Source 1)](#90-empirical-vs-modeled-data-source-1). Code 1
    (Empirical) and Code 2 (Modeled) **are mutually exclusive.**

6.  **Primary vs Secondary**: In this column, AI must record the most
    accurate code or codes from the Primary vs Secondary (Data Source 2)
    code typology provided in section [10.0 Primary vs Secondary (Data
    Source 2)](100-primary-vs-secondary-data-source-2). Code 1 (Primary)
    and Code 2 (Secondary) **are mutually exclusive.**

7.  **Asked/stated vs Measured/observed (Data Source 3)**: In this
    column, AI must record the most accurate code or codes from the
    Asked/stated vs Measured/observed (Data Source 3) code typology
    provided in section [15.0 Asked/stated vs Measured/observed (Data
    Source 3)](150-asked-stated-vs-measured-observed-data-source-3).
    Code 1 (Asked/stated) and Code 2 (Measured/observed) **are mutually
    exclusive.**

8.  \*\* Target Population/Data Collection Rationale (Consolidated)**: A
    unified rationale justifying the codes selected in Column 1
    (**Community Type**), Column 2 (**Unit of Observation**), Column 3
    (**Unit of Analysis**), Column 6 (**Empirical vs Modeled**), Column
    7 (**Primary vs Secondary**), and Column 8 (**Asked/stated vs
    Measured/observed\*\*).

9.  **Aquaculture Relevance Code**: In this column, the AI must assign
    one or more numerical codes (1, 2, 3, or 4) or "n/a" that accurately
    reflect the indicator's thematic or methodological relationship to
    the aquaculture context as described in the source article. The
    typology is defined as follows:

| Code | Relevance Description                              | Definition                                                                                                                                                                                                                                                                                                                                                                            |
|:--------------------------:|:---------------------|:---------------------|
|  1   | Applied to evaluate an aquaculture context         | The indicator was explicitly measured or scored within the current study to evaluate the performance or status of a real-world aquaculture case, project, or system (e.g., scoring a salmon farm's profitability).                                                                                                                                                                    |
|  2   | Developed for future use in an aquaculture context | The study's primary objective or major recommendations section focuses on proposing or testing the metric's methodological validity for assessing aquaculture (e.g., building a new fish health index for aquaculture; informing recommendations, development strategies, or scenario planning specifically targeting the growth, viability, or scaling up of the aquaculture niche). |
|  3   | Some other relevance                               | The indicator is a direct methodological analog (structurally identical/transferable) to a core aquaculture metric OR provides essential socio-economic/environmental context for the aquaculture niche, even if not explicitly used for aquaculture planning in the study.                                                                                                           |
|  4   | Tangential other                                   | The indicator's relevance is purely external or incidental to the primary findings and methodology of the study, and is noted only for compliance or high-level thematic completeness.                                                                                                                                                                                                |
| n/a  | Not relevant                                       | The indicator is exclusively focused on a competing, specific non-aquaculture methodology (e.g., specific capture gear types, capture stock status) and offers no significant contextual overlap or direct methodological transferability.                                                                                                                                            |

**Non-Exclusivity Rule**: Codes 1, 2, 3, and 4 are not mutually
exclusive and should be listed together (e.g., "1; 2; 3") if applicable.

10. **Aquaculture Code Rationale**: In this column, the AI must provide
    a concise justification for the assignment of the Aquaculture
    Code(s) in the preceding column. The rationale must explicitly
    connect the selected code(s) to the indicator's purpose, the
    research findings, or the recommendations regarding the aquaculture
    niche in the source article. Format Constraint: The rationale should
    briefly state the indicator's role (e.g., "Measures direct
    investment constraint on fish farming," or "Indicator is a
    macro-economic driver whose negative outcome (low prices) constrains
    the aquaculture niche").

## **16.9 Table 8 Specifications (Conceptual Topic and Feedback)**

Using the same list of indicators generated in Table 1, the AI must
populate Table 8 by compiling the final data on the Indicator Topic and
all associated qualitative feedback from Table 3. Creation of Table 8
must follow the Validation Rule in section [16.1 Rules for All
Tables](#160-rules-for-all-tables).

### **16.9.1 Table 8 Column Specifications**

The AI must use the same indicator order and numbering for Table 8 as
was included in the final Table 1 output. Following the column with the
indicator name, the following attributes must each be included in their
own column:

**Sub-category (Indicator Topic)**: The exact wording of the conceptual
sub-category representing the indicator's **conceptual representation
target**, compiled from Tables 3 and 4.

**Definition Match (Indicator Topic)**: The specific words or phrases
from the source text that justify the sub-category selection for the
indicator topic, including any required suggestions for additions to the
definition (see Protocol 16.3.1).

**Conceptual Distinction Issues (Indicator Topic)**: The documented
qualitative feedback describing any ambiguity, lack of clarity, or
conceptual overlap encountered during matching, compiled from Tables 3
and 4.

**Suggested Definition Edits (Indicator Topic)**: The actionable advice
and specific text modifications intended to resolve ambiguities or
overlaps in the GIP's typology, compiled from Tables 3 and 4.

**Sub-category (Primary Variable Concept)**: The exact wording of the
conceptual sub-category representing the indicator's **primary
conceptual assessment target**, compiled from Tables 3 and 4.

**Definition Match (Primary Variable Concept)**: The specific words or
phrases from the source text that justify the sub-category selection for
the primary variable concept, including any required suggestions for
additions to the definition (see Protocol 16.3.1).

**Conceptual Distinction Issues (Primary Variable Concept)**: The
documented qualitative feedback describing any ambiguity, lack of
clarity, or conceptual overlap encountered during matching, compiled
from Tables 3 and 4.

**Suggested Definition Edits (Indicator Topic)**: The actionable advice
and specific text modifications intended to resolve ambiguities or
overlaps in the GIP's typology, compiled from Tables 3 and 4.

# **17.0 Visual Decision Trees**

## **17.1 Decision Tree for Determining Indicator Inclusion**

-   Is the variable used for a management purpose?

-   Yes

-   Is the variable separately described?

-   Yes

-   Include as indicator

-   No

-   Exclude unless at least one basic component is present

-   No

-   Exclude

## **17.2 Decision Tree: Assigning Variable Type (Pre-Scoring, Scoring, and Outcome)**

**PART A: Determining Pre-Scoring vs. Scoring Variable Types** - **Step
1: Is the variable directly assessed?** - **No (Aggregate/Composite)**
──\> - **Pre-Scoring**: Write "see sub-variables". - **Variable Type
Upon Scoring**: Write "see sub-variables". - **Yes (Raw Indicator)**
──\> Proceed to Step 2.

-   **Step 2: Determining Pre-Scoring vs. Scoring for Raw Indicators**
    -   Identify the data type used to perform the actual
        assessment/score (e.g., the 1-5 scale, the Nominal category).
        This is the **Variable Type Upon Scoring**.
    -   **Was the raw data transformed to reach this state?** (e.g., raw
        narrative coded into a rank, or continuous values binned).
        -   **No (Identical state)** ──\> **Pre-Scoring**: Write "n/a".
        -   **Yes (Transformation occurred)** ──\> **Pre-Scoring**:
            Assign the data type of the raw, original state.

**PART B: Determining Variable Type of Outcome** - Does the assessment
result in a calculated value, category, or summary that is distinct from
the individual indicator score? - **No** (The indicator score is the
final output) ──\> Variable Type of Outcome is **n/r**. - **Yes**
(Aggregation results in a new value) ──\> Assign the data type of the
**final resulting value** (e.g., the final Composite Score type).

**PART C: Assigning Outcome Type (Codes 5-12)** - Does the variable
represent a summary, aggregate, or mathematical transformation? - **No**
──\> Outcome Type is **n/r**. - **Yes** ──\> Select all that apply: 1.
**Complex Modeling**: Produced via statistical estimation/simulation?
──\> **Code 10**. 2. **Aggregation**: Combines 2+ distinct variables?
──\> **Apply Section 17.6** (for Code 6 vs. 11). 3. **Derived Math**:
Simple ratio or structural calculation? ──\> **Code 8**. 4.
**Descriptive**: Summary of population (count, mean, %)? ──\> **Code
5**. 5. **Narrative**: Non-quantified conceptual effect? ──\> **Code
12**.

## **17.3 Decision Tree for Selecting Appropriate Sub-category for Variable Concept**

-   Start

-   Is the variable directly assessed (i.e., the variable type upon
    scoring is identified, and does not say "see sub-variables")?

-   Yes

-   Based on primary and sub-category definitions provided in the
    section "Conceptual categories," identify:

-   The primary category that is the best match for the variable concept

-   The sub-category that is the best match for the variable concept

-   Write the sub-category name (only the portion of the category name
    after the colon) in the "Sub-category of variable concept" column.

-   No

-   Write "n/r" in the column "Sub-category of variable concept"

## **17.4 Decision Tree: Selecting Appropriate Sub-category for Indicator Topic**

-   Start

-   Does the research provide information about the topic the indicator
    is meant to represent?

-   Yes

-   Based on primary and sub-category definitions provided in the
    section "Conceptual categories," identify:

-   The primary category that is the best match for the indicator topic

-   The sub-category that is the best match for the indicator topic

-   Write the sub-category name (only the portion of the category name
    after the colon) in the "Sub-category of indicator topic" column.

-   No

-   Write "n/r" in the column "Sub-category of indicator topic"

## **17.5 Decision Tree for Determining if a Conceptual Proxy is Present**

-   Start

-   Does the "Sub-category of variable concept" say "see sub-variables?"

-   Yes

-   Write "n/a" in the column "Conceptual Proxy Present."

-   No

-   Is the sub-category listed in the column "Sub-category of variable
    concept" the same as the sub-category name listed in the column
    "Sub-category of indicator topic"?

-   Yes

-   Write "n/a" in the column "Conceptual Proxy Present."

-   No

-   Write "Yes" in the column "Conceptual Proxy Present."

## **17.6 Decision Tree: Distinguishing Outcome Types 5, 6, 7, 8, 11, and 12**

**START: Is the indicator a qualitative response variable (Y) asserted
to be influenced by an element (X) within a Narrative Causal
Statement?** - **YES** ──\> **CODE 12: Narrative Causal Outcome** -
**NO** ───\> Proceed to Step 1.

**STEP 1: Multi-Faceted Conceptual Test** **Does the indicator represent
a "higher-order" concept created by fusing multiple, conceptually
heterogeneous facets?**

-   **NO (Functional or Structural Operation)**: The calculation is a
    mathematical translation for utility or a tally of related physical
    units.
    -   **Examples**:
        -   **Standardization**: Converting a value to a **Z-score** or
            0--1 scale.
        -   **Functional Ratio/Rate**: Calculating **CPUE**
            (Catch/Effort) or **Density** (Fish/Area).
        -   **Structural Tally**: Summing components of the same
            physical category (e.g., **Total Assets** = Gear + Boat +
            Engine).
    -   **Action** ──\> **Proceed to Step 3**.
-   **YES (Conceptual Fusion)**: Disparately different dimensions (e.g.,
    "Income" + "Health" + "Political Voice") are joined to represent a
    theoretical or complex state (e.g., "Well-being" or
    "Vulnerability").
    -   **Action** ──\> **Proceed to Step 2**.

**STEP 2: Direction of Causality Test (For Multi-Faceted Concepts)** -
**PATH A: Parts → Whole (Constitutive)**: The sub-variables are building
blocks that define the concept. If a part is removed, the concept is
redefined or becomes incomplete (e.g., Vulnerability Index). -
**RESULT** ──\> **CODE 6: Composite Index** - **PATH B: Whole → Parts
(Reflective)**: The sub-variables are manifestations or "symptoms" of an
unobservable latent state (e.g., Social Capital). - **RESULT** ──\>
**CODE 7: Latent Construct**

**STEP 3: Single-Concept Test (For Non-Faceted/Structural Outcomes)** -
**Is the result a population-level summary of a single attribute across
many units (e.g., Mean, Median, Count, Percentage)?** - **YES** ──\>
**CODE 5: Descriptive Statistics** - **Is the result a functional math
transformation or a structural/cumulative total of related units?** -
**Diagnostic**: Does it represent a ratio, a standardized score, or a
tally of physical units without creating a new multifaceted
"theoretical" concept? - **YES** ──\> **CODE 8: Other Derived
Outcome** - **If neither apply**, proceed to Step 4.

**STEP 4: Identity Test** **Is the primary purpose to identify an
Identity Type, Regime, or Typology?** - **Diagnostic**: Does the result
describe a **kind** of system based on a mix of attributes (e.g.,
"Industrial vs. Artisanal") rather than an aggregate score of a complex
concept? - **YES** ──\> **CODE 11: Categorical Outcome** - **NO** ───\>
**CODE 9: Unknown Outcome Type**.

**[RECONCILIATION RULE]**: 1. **FRAME OVER FORM**: If a variable
summarizes aggregate status or a conceptual representation (e.g.,
"Sustainability Rank"), the **Constitutive Mandate of Code 6** takes
precedence over Code 11 or Code 8, regardless of the output data type.
2. **MODEL PROVENANCE**: If any outcome (5, 6, 7, 8, or 11) is produced
via statistical simulation/estimation rather than simple arithmetic, it
**MUST** be dual-coded with **Code 10 (Model Output)**.

# **18.0 Prompts for Producing and Validating AI Table Outputs**

| Prompt number | Title of Prompt | Prompt instructions |
|:---:|:---|:---|
| **P1** | **REVIEW GIP & OPERATIONAL PILLARS** | "The AI must review and confirm comprehension of the full Global Instruction Preamble (GIP). In your confirmation, you must explicitly acknowledge and commit to the following five Operational Pillars to ensure consistency throughout the study:<br><br>1. **Foundation Integrity (P1–P14)**: You will strictly apply the Narrative Purity Constraint (2.1.7), Parameter Inclusion Criterion (2.1.2), and Dual VAD Mandate (2.1.5) to define the master indicator pool before mapping begins.<br>2. **Immutable Data Lock (P15)**: You acknowledge that upon the execution of P15, the indicator pool (IDs and Names) becomes immutable. No indicators shall be added, renumbered, or deleted after this point to protect relational integrity.<br>3. **Relational Precision (Table 2)**: You must distinguish between constitutive and predictive links, explicitly categorizing rationales as 'Structural-Only,' 'Causal-Testing,' or 'External Causal' per Rule 16.3.2.5.<br>4. **Just-in-Time Re-scans (P26 & P32)**: You are required to re-read the specific table specifications in Sections 16.8 and 16.9 immediately before generating Tables 7 and 8 to prevent context drift.<br>5. **Technical Rigor**: All outputs must be valid pipe-delimited tables. Every cell intended for rationale or feedback must contain the 'n/a' placeholder if no entry is required; no cells may be left blank.<br><br>Confirm your comprehension and readiness to proceed according to these specific pillars." |
| **P2** | **REQUEST ARTICLE TEXT** | "AI must request the text of a new article for review." |
| **P3** | **REQUEST SUPPLEMENTAL MATERIAL TEXT** | "AI must request any relevant supplemental materials, if available." |
| **P4** | **PRODUCE TABLE 1 (Initial)** | "AI must produce Table 1, following instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes)." |
| **P5** | **REQUEST HUMAN INDICATOR LIST** | "AI must request the list of indicators produced by the human research team, and once the list is received AI must recreate Table 1 with two extra columns, one with the indicator ID number (XXXX&#95;X) given by the human research team, and one with the name given to the indicators by the human research team. The AI must match the human indicators to the original AI-generated list of indicators, revising the internal numbering of the original AI-generated indicator list to match the numbering of the human generated list. The AI must refresh its internal numbering of indicators using the strict rule that the AI's numbering system must match the final digits of the human-generated indicator ID (i.e., the digit(s) following the underscore, “&#95;X”). If the human research team's list includes indicators that were not included on the original AI-generated list, the AI must write \"n/a\" in the AI indicator name column and must include these indicators when populating all attributes columns. If the original AI-generated list of indicators includes an indicator that the human research team did not identify, the AI must write \"n/a\" in the new columns for Human indicator ID and human-assigned indictor name. The AI must sort the list in the order of the human indicator ID, with any of additional indicators added by the AI list at the bottom of the list, numbered in continuation from the end of the human-generated list of indicator ID numbers (e.g., if the final human-generated indicator ID ends in \"&#95;20,\" any additional indicators from the AI-generated list would start with \"21\" and continue on with \"22\" etc. until the final AI-generated indicator has been numbered." |
| **P6** | **MANDATORY NARRATIVE CAUSAL STATEMENT (NCS) CHECK** | "The AI must perform a comprehensive audit of the qualitative results and discussion sections to identify all explicit statements asserting a systemic, directional causal influence (X -> Y).<br><br>STRICT SOURCE CONSTRAINT: Pursuant to Section 3.1 (Code 4) and Rule 2.1.7 (Narrative Source Purity), a variable may ONLY be coded as Narrative (Code 4) and included as part of an NCS if it is substantiated by findings derived from raw qualitative data arising from direct engagement with human subjects (e.g., interview transcripts, field notes, observation logs).<br><br>MANDATORY EXCLUSION: Pursuant to Rule 2.1.6, the AI must explicitly exclude any causal relationships derived from the authors' historical method, discourse analysis of administrative/legal documents, or synthesis of quantitative trends, as these do not constitute 'Narrative' variables under this framework.<br><br>Mandate: For every unique NCS identified that passes the source constraint, the AI must ensure both the Narrative Causal Element (NCE, X) and the Narrative Causal Outcome (NCO, Y) are included in the indicator list as distinct indicators, even if not otherwise separately detailed.<br><br>Coding Verification: For all new and existing NCS indicators, verify compliance with the GIP:<br>1. NCE (X): -> Variable Type Upon Scoring = 4 (Narrative); Outcome Type = n/r.<br>2. NCO (Y): -> Variable Type Upon Scoring = 4; Outcome Type = 12 (Narrative causal outcome); Variable Type of Outcome = 4.<br>3. Inclusion Justification: Must be coded as 4 (Inferred (Narrative)).<br><br>Provide a rationale for any identified causal statements in the text that were REJECTED based on the Narrative Synthesis Exclusion (Rule 2.1.6), provide a rationale for any new additions or coding changes for accepted statements, and then present the final, validated Table 1 output." |
| **P7** | **DOUBLE CHECK PARAMETER INCLUSION CRITERIA** | "The AI must audit Table 1 for all indicators identified as parameters used in a formula or model, particularly those with Inclusion Justification Code 3 (Inferred) or Code 2 (Score Only). Verify strict compliance with the Parameter Inclusion Criterion (Rule 2.1.2): AI should not include **parameters** in the list of indicators **unless the parameter is actively estimated, calibrated, or set using real-world data specifically for the study's contextual or baseline assessment**. This includes parameters estimated by minimizing log likelihoods, setting to observed baseline averages, derived from secondary sources where the specific value is selected, spatially or temporally calibrated, or adjusted to fit the study's unique geographical, environmental, or baseline conditions, or otherwise adjusted to anchor the model to the local case study. Parameters treated as global, fixed constants with no contextual specificity must be removed (e.g., 'Indicator 4: Mortality Rate removed. Rationale: Sourced as a fixed constant from Smith et al. (2010), not estimated by the current study'), and provide a revised Table 1 output." |
| **P8** | **SECTION 2.1 INTEGRITY AUDIT** | "The AI must perform a final audit on Table 1 to ensure full compliance with all Indicator Inclusion Constraints (Section 2.1), serving as a crucial verification step before entering the relationship mapping phase. Specifically, the AI must verify compliance with the following rules:<ul><li>Rule 2.1.2 (Parameter Inclusion Criterion): Confirm fixed, unadjusted constants sourced from literature have been correctly removed.</li><li>Rule 2.1.4 (Narrative Causal Statement Mandate): Confirm all NCE/NCO variables are included and coded as Narrative (Code 4) and Outcome Type 12.</li><li>Rule 2.1.5 (Dual VAD Separation Mandate): Confirm that concepts assessed by both quantitative and narrative VADs are listed as two separate, non-constitutive indicators.</li><li>Rule 2.1.7 (Narrative Synthesis Requirement): Confirm the methodological integrity of all Narrative Variables (Code 4) by verifying that the variable is the product of the study's direct synthesis of raw qualitative data (as defined in 2.1.7) and not the citation of a pre-existing summary or finding synthesized by a third party.</li></ul>List any indicator changes or coding corrections with rationale, and provide the final, validated Table 1 output." |
| **P9** | **MANDATORY DESCRIPTIVE GROUPING CHECK (MDGC)** | "AI must perform a Mandatory Descriptive Grouping Check (MDGC) to ensure all essential nominal grouping variables are included as explicit indicators for subsequent X-Y relationship mapping, preventing exclusion errors. 1. **Identify Core Segmentation:** Scan the Indicator Name and Source Context of all quantitative indicators (those with Outcome Type Code 5 or 8) to identify implicit nominal variables used for systematic data segmentation (e.g., separating data by Country, Fishing-Practice Group, or Aquaculture Environment). 2. **Flag Grouping Variables:** If a quantitative indicator (Y) consistently presents aggregated results segregated by an implicit nominal variable (X) across multiple tables/sections, the nominal variable (X) must be immediately flagged. This confirms (X) functions as a primary **Relating Variable (X)**. 3. **Enforce Inclusion:** If a flagged nominal variable (X) is not already listed, the AI must: a. **Insert it** into the indicator table as a new entry. b. Assign **Variable Type upon Scoring = 3 (Nominal)**. c. Assign **Outcome Type = n/r**. d. Assign **Inclusion Justification = 1 (Named/Defined)**. 4. **Provide Revised Table 1 and Rationale:** List the newly added indicator IDs and their rationale (e.g., \"Added Variable [X], [Group Name], due to its systematic use in segmenting Indicators [Y1, Y2, Y3] across multiple tables/figures.\"). Provide the final, revised Table 1 output." |
| **P10** | **DOUBLE CHECK TABLE 1 AGAINST VARIABLE TYPE RULES** | "The AI must re-verify that the entries in the **Variable Type upon Scoring** and **Pre-scoring Variable Type** columns in Table 1 have been populated correctly with reference to the Secondary rule. Please also re-verify the entries in the **Outcome Type** column in Table 1 to ensure that the assignments reflect the strict definitional distinctions between outcome types: **Composite index (6)** code, **Latent construct (7)** code, **Other derived outcome (8)** code, **Model output (10)** code, and **Categorical outcome (11)** code. Also verify the correct application of the **Model output (10)** code, ensuring it is inherited by all downstream calculated indicators that use a Model Output as an input. Please confirm if any changes are required, list the changes with rationale, and provide a revised Table 1 output." |
| **P11** | **DOUBLE CHECK TABLE 1 INCLUSION JUSTIFICATION COLUMN** | "The AI must audit the **'Inclusion Justification'** column of Table 1. For any indicator marked **'Inferred (SADP),'** confirm the following: (1) It lacks both a 'Named/Defined' status and a 'Score Only' status, AND (2) Its inclusion is strictly justified by the **Hierarchical Constitutive Exception** (i.e., it is essential for completing a single-step link between two other described/scored indicators). Please confirm if any changes are required, list them with rationale, and provide a revised Table 1 output." |
| **P12** | **VALIDATION CHECK ON CATEGORICAL INDICATOR INTEGRITY** | "This protocol ensures that nominal and categorical variables are correctly represented.<br><br>### 1. Nominal Label Exclusion Test (Consolidation Mandate)<br>Audit all indicators to ensure no two or more items represent the mutually exclusive states (labels) of a single nominal variable (e.g., Policy Scenario A, Scenario B). Consolidation is required if variables have an identical concept, non-calculated input/setting role, and pass the following criteria:<br>• **Pass Condition:** The variable must be simple (not derived/calculated) and multiple entries must map to the exact same conceptual sub-category.<br>• **Action:** Merge the labels into one single categorical indicator entry (e.g., 'Policy Scenario Type').<br><br>### 2. Essential Nominal Indicator Inclusion Test (Inclusion Mandate)<br>Audit the study's primary analyses to identify any Nominal Variable that functions as a core Target Variable (Y) or a critical, non-calculated Relating Variable (X).<br>• **Action:** If missing, include as a new entry (Variable Type -> Code 3).<br><br>### 3. Categorical Outcome Mandate (Code 11 Check)<br>Audit all included nominal/categorical variables (Code 3) against the Categorical Outcome Mandate (Section 3.2, Code 11): Apply Code 11 to high-level classifications used in comparative analysis where the classification represents an aggregation of complex characteristics.<br>• **Action:** If the variable is a high-level aggregate, recode the Outcome Type to Code 11 and ensure Variable Type columns are set to 'see sub-variables.'<br><br>If changes are required, list them with rationale and provide a revised Table 1 output." |
| **P13** | **MANDATORY EXCLUSION LOGIC TEST** | "Identify and list three specific examples from the raw supplemental data where an item was NOT consolidated into a higher-level Composite Index (Code 6) or the Categorical Outcome (Code 11). For each example, explicitly state which clause of the Measurement Component Inclusion Mandate (16.2.1.2 a or b) prevents its consolidation, confirming that the new rule is being applied correctly to retain granular VAD data." |
| **P14** | **DUAL VAD SEPARATION AND CODING AUDIT** | "Perform a mandatory audit to confirm the correct implementation of the **Dual Variable Assessment Detail (VAD) Distinction Mandate (Rule 2.1.5)**. Specifically, audit the indicator list to identify any concepts that are assessed using two fundamentally distinct Variable Assessment Details (VADs) that lead to a difference in the fundamental variable type (Codes 1-4). 1. **Separation Check**: Confirm that any concept with both a Quantitative VAD and a Qualitative/Narrative VAD is listed as two distinct indicators. 2. **Quantitative VAD Coding**: Confirm the quantitative indicator is correctly coded to reflect its VAD (Code 1, 2, or 3) and n/r Outcome Type. 3. **Narrative VAD Coding**: Confirm the narrative indicator is correctly coded to reflect its narrative VAD (Code 4) and appropriate Outcome Type (Code 12 or n/r). List any discrepancies and provide the corrected Table 1." |
| **P15** | **FINAL TABLE 1 LOCK AND VALIDATION** | "The AI must perform a final, comprehensive audit to synchronize the human-assigned indicator list (from P5) with the AI's current validated list (incorporating all corrections from P6–P14).<br><br>1. **Indicator Sync**: Verify that every Indicator ID and Name matches the sorted human/AI merged list exactly.<br>2. **Final Variable Type Audit**: Re-confirm that every 'Outcome Type' reflects the strict definitional distinctions (Codes 6, 7, 8, 10, or 11) and that 'see sub-variables' is correctly applied in the 'Variable Type Upon Scoring' and 'Pre-scoring Variable Type' columns.<br>3. **The Lock**: Present the definitive, final version of Table 1. Explicitly state: 'This version of Table 1 is now the immutable reference for all downstream tables. No indicators will be added, removed, or renumbered after this point.'<br>4. **State Refresh**: Briefly summarize the Column Specifications for Table 2 (Section 16.3.2) to ensure active comprehension before proceeding." |
| **P16** | **PRODUCE TABLE 2 (WITH X-Y VALIDATION)** | "Using the same list of indicators in the same order as Table 1, the AI must produce Table 2, following instructions in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes). **Immediately following table creation, the AI must perform a validation audit:** For all entries in the **Target variable** and **Relating variable** columns of Table 2 where a relationship code (1-9) is present, the AI must explicitly document the model's **directionality** (Directional/Non-Directional) and its final **statistical finding** (Significant/Not Significant) as derived from the source text or outputs, and verify that the resulting relationship code aligns exactly with the definitions and protocols in Section 14.3.2. List any identified errors and corrections with rationale, and then present the final, validated Table 2." |
| **P17** | **CATEGORICAL LINK STRUCTURAL INTEGRITY CHECK** | "The AI must audit Table 2 to ensure all **Constitutive Links** are strictly excluded from the predictive columns (Target/Relating). Specifically: **Mandate**: For any Indicator (Y) whose **Outcome Type** in Table 1 is Code 11 (Categorical Outcome), and whose link (X $\to$ Y) is designated as constitutive (X is listed in the Associated Sub-variable column of Y): 1. The **Relating variable** column for Y MUST be set to 'n/a' (or contain only non-constitutive links). 2. The **Target variable** column for X MUST be set to 'n/a' (or contain only non-constitutive links). List any identified constitutive link (X $\to$ Y) that was incorrectly included in the predictive columns with rationale (Rule 14.3.1 Exclusion) and provide the corrected Table 2 output." |
| **P18** | **CONSTITUTIVE FLOW AND STRUCTURAL INTEGRITY AUDIT** | "Audit Table 2 to verify the integrity of the constitutive indicator chain and structural rules, applicable to any article: 1. Immediate Constitutive Link Rule Check: Confirm strict adherence to the **Immediate Constitutive Link Rule** (14.2.2). Verify that input sub-variables link only to their direct aggregate outcome variable, and that aggregate variables (e.g., intermediate indices) are correctly chained up to the final highest-level outcome variable. 2. Narrative/Quantitative Separation Check: Confirm that indicators whose Variable Type Upon Scoring is **Narrative (Code 4)** are **entirely absent** from the Associated Outcome Variable and Associated Sub-variable columns. (They must only appear in the predictive columns, per the structural exclusion mandate and Rule 2.1.5). 3. Synchronization Mandate Check: Confirm that every input sub-variable is correctly assigned the corresponding **Conceptual Relationship Code** (Code 3, 4, or 5) in Table 4 (when produced), based on the final Outcome Type of its immediate Associated Outcome Variable (Codes 7, 6, or 8/11, respectively). List any identified errors and provide the corrected Table 2." |
| **P19** | **PRODUCE TABLE 3** | "Using the same list of indicators in the same order as Table 1, the AI must produce Table 3, following instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes)." |
| **P20** | **PRODUCE TABLE 4** | "Using the same list of indicators in the same order as Table 1, the AI must produce Table 4, following instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes)." |
| **P21** | **PRODUCE TABLE 5** | "Using the same list of indicators in the same order as Table 1, the AI must produce Table 5, following instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes). **MANDATORY VALIDATION STEP:** The AI must audit the **Conceptual Proxy Present** column to ensure strict compliance with the **Inclusion Constraint (Derived Indicators)** (Section 16.6.1, Column 1). Specifically, if the indicator's **Outcome Type** (Table 1) is Code **6, 7, 8, 10, or 11**, the **Conceptual Proxy Present** column **MUST be set to \"n/a\"** regardless of any comparison between the Primary Variable Concept and the Indicator Topic. Provide a revised Table 5 output if corrections were required." |
| **P22** | **PRODUCE TABLE 6** | "AI must re-read Section [16.7 Table 6 Specifications](#167-table-6-specifications) and then produce Table 6 using the same list of indicators in the same order as Table 1. In producing Table 6, the AI must also follow general instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes). Ensure the 'Rationale' column citations strictly use Indicator numbers (e.g., 'sub-variable of 24') and specify the exact GIP rule number applied for each code." |
| **P23** | **COMPLEX LOGIC CHECK: DESCRIPTIVE STATS INTEGRITY** | "The AI must audit all indicators in Table 6 for compliance with the **Descriptive Statistics Integrity Rules** concerning Outcome Type Code 5 (Descriptive statistics):<br><br>1. **Code 6 Exclusion Mandate:** For every indicator with Outcome Type Code 5 in Table 1, verify that **Code 6** (Outcome variable) is **NOT** present in the **Conceptual Relationship Code** column in Table 4 (Section 4.2 constraint).<br><br>2. **Code 1/2 Priority Mandate:** For every indicator with Outcome Type Code 5 in Table 1 and **n/a** in the **Associated Sub-variable** column in Table 2, confirm that the **Conceptual Relationship Code** in Table 4 is either **1** or **2** (and not **7**), depending on the conceptual proxy status in Table 5 (Section 4.2 priority rule).<br><br>Provide a rationale for any discrepancies found and a final, corrected Table 6 output." |
| **P24** | **CONCEPTUAL PURITY CHECK (CODE 1 EXCLUSIVITY)** | "The AI must audit Table 6 for all instances where Conceptual Relationship Code 1 co-occurs with any other conceptual relationship code (Codes 2, 3, 4, 5, 6, or 7). **Mandate for Code 1 Exclusion**: Pursuant to the Co-occurrence Rules in Section [4.2 Conceptual Relationship Typology](#42-conceptual-relationship-typology), Code 1 is strictly prohibited from co-occurring with any other code. For every instance of co-occurrence found, the AI must immediately correct Table 6 by **removing Code 1** from the entry, retaining only the remaining code(s) (e.g., changing '1; 4' to '4'). This correction enforces the definition that Code 1 applies only to indicators that are **NOT a constitutive sub-variable.** Provide a brief rationale for the correction and present the final, validated Table 6 output." |
| **P25** | **COMPREHENSIVE CONCEPTUAL RELATIONSHIP AUDIT** | "Audit Table 6 to verify the integrity of all Conceptual Relationship Codes (1-7) against the GIP definitions:<br><br>1. **Constitutive Synchronization Check (Codes 3, 4, 5 Priority)**: Confirm all sub-variables in Table 2 are assigned the correct input code (3, 4, or 5) in Table 6, explicitly synchronized with the Outcome Type (6, 7, 8, or 11) of its immediate Associated Outcome Variable in Table 1.<br>2. **Outcome Status Check (Code 6/7/8/11)**: Confirm Code 6 (Outcome variable) in Table 6 is assigned ONLY to indicators whose Outcome Type in Table 1 includes Code 6, 7, 8, or 11.<br>3. **Single Variable Status Check (Codes 1 & 2)**:<br>• Confirm Code 1 is assigned ONLY to non-constitutive indicators where the PVC and Indicator Topic are identical.<br>• Confirm Code 2 is assigned ONLY to non-constitutive indicators where a proxy is present.<br>• **Univariate Transformation Guardrail**: Pursuant to Section 3.2.1.1, verify that indicators representing a single variable that has been re-binned or transformed are NOT assigned Outcome Type 6, 7, 8, or 11.<br>4. **Exclusion Check (Code 1)**: Confirm Code 1 is strictly prohibited from co-occurring with any other constitutive code (Codes 3, 4, 5, 6, 7).<br><br>List any discrepancies and provide the corrected Table 6 output." |
| **P26** | **PRODUCE TABLE 7** | "AI must re-read Section [16.8 Table 7 Specifications](#168-table-7-specifications) and then produce Table 7 using the same list of indicators in the same order as Table 1. In producing Table 7, the AI must also follow general instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes)." |
| **P27** | **TABLE 7 CONSISTENCY AND EVALUATION VALIDATION** | "**Mandate 1 (No Inference Rule)**: Audit Table 7 to confirm every entry in the **Community Type, Unit of Observation, Unit of Analysis, Empirical vs Modeled, Primary vs Secondary, and Data Source 3** columns strictly adheres to the rule that if information is unknown, the code \"n/r\" or \"Undetermined\" is used, rather than inferring data types or scales not documented in the source text. **Mandate 2 (Evaluation Verification)**: Audit the **Indicator Action** column for all instances of Code **1 (Evaluation)**. Verify the indicator was demonstrably used in an assessment of a real-world system, as defined in section [8.0 Indicator Action](#80-indicator-action). If the sole purpose was purely theoretical, Code 1 must be removed. List any discrepancies and provide the corrected Table 7 output." |
| **P28** | **CALCULATION FLOW CHART GENERATION PROMPT** | "Based exclusively on the data in the **'Associated Sub-variable'** and **'Associated Outcome Variable'** columns, generate a complete flow chart detailing the calculated relationships. The output must adhere strictly to the following format:<br>1. **Format:** A single, pipe-delimited table suitable for Excel.<br>2. **Sectioning:** Group calculation chains logically. Use title format: **X. [Index Name] Chain (#[Index ID]).**<br>3. **Section Divider:** Use a row of `---` between sections.<br>4. **Content:** Table must contain six columns: 1. Flow Chart Section; 2. Sub-Variable (Input); 3. Status (N, S, I); 4. Conceptual Relationship Code; 5. Formulaic Link; 6. Outcome Variable.<br>**Note:** Ensure every constitutive link is represented once." |
| **P29** | **Verify Conceptual Relationship Typology** | "Verify that the conceptual relationship code populated in the calculation flow chart relied on the **Conceptual Relationship Typology (Codes 1–7)** from section [4.2 Conceptual Relationship Typology](#4.2-conceptual-relationship-typology) of the Global Instruction Preamble (GIP)." |
| **P30** | **X-Y Relationship Flow Chart Generation Prompt** | "Create a similar flow chart for relating variables to target variables, with the following specifications:<br><br>1. **Status (N, S, I)**: Use the correct code from the Inclusion Justification for the status of the Relating Variable (X). (Rationale: Ensures consistency in detailing origin).<br>2. **X-Y Relationship Code**: The Conceptual Code column must use the **X-Y Relationship Type Code (1-9)**, not the Constitutive Link Code (3, 4, 5). (Rationale: Clarifies distinction between causal (X-Y) and mathematical (Constitutive) one)." |
| **P31** | **Verify X-Y Relationship Typology** | "Verify that the X-Y relationship flow chart relied on the **Predictive X-Y relationship codes (Codes 1–9)** from section [14.3.2 X-Y Relationships to Record](#1432-x-y-relationships-to-record) of the Global Instruction Preamble (GIP)." |
| **P32** | **PRODUCE TABLE 8** | "AI must re-read Section [16.9 Table 8 Specifications (Conceptual Topic and Feedback)](#169-table-8-specifications-conceptual-topic-and-feedback) and then produce Table 8 using the same list of indicators in the same order as Table 1. In producing Table 8, the AI must also follow general instruction in Section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes)." |
| **P33** | **GLOBAL TABLE OUTPUT FINALIZATION AUDIT** | "The AI must perform a **Global Table Output Finalization Audit** on Tables 1 through 8 to ensure compliance with the **Rules for All Tables** in section [16.0 Instructions for Producing Tables of Indicators and their Attributes](#160-instructions-for-producing-tables-of-indicators-and-their-attributes). Specifically: **1. Structural Integrity Check:** Verify correct column structure and pipe alignment. **2. Placeholder Compliance Check:** Verify every rationale/feedback cell is populated with substantive text or the placeholder **\"n/a\"**, ensuring no blank cells exist. List location errors found and provide a statement confirming compliance." |
| **P34** | **PRODUCE RATIONALE AND ANALYTICAL ROLE MAPPING** | "The AI must produce a final 'Indicator Rationale and Analytical Role Mapping' table for all indicators. 1. **Ordering & Grouping**: Indicators must be listed in the exact same numerical order as Table 1; within that sequence, identify their position in the constitutive hierarchy (e.g., Final Outcomes, Sub-Aggregates, Constitutive Inputs, Empirical Anchors, and Predictive Relaters). 2. **Columns**: Include Indicator #, Name, Inclusion Justification (Code/Text), Analytical Role, and a Rationale for Inclusion & Role in the Analysis. 3. **AI Note Mandate**: Every rationale entry MUST begin with the prefix **'AI note: '**. 4. **Content**: Explain the 'why' (GIP mandate) and the 'how' (specific role in the study's mathematical or causal logic). 5. **Validation**: Ensure every indicator from Table 1 is represented consistently." |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
