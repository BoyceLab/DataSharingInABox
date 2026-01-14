---
title: Data Sharing Readiness Assessment
toc: true
---

## ✅ Data Sharing Readiness Assessment

!!! tip "Purpose of This Checklist"
    This page helps registry holders, patient advocacy groups, and data stewards assess their **data sharing readiness** including documentation, governance, technical infrastructure, and **data standardization**.

    It is especially useful for registries that include **multiple data sources** (e.g., EHR, surveys, biosamples, imaging, genomics) and want to prepare for **external data sharing, harmonization, or OMOP mapping**.

---

## 🧭 How to Use This Page

This assessment is organized into **three layers**:

1. **Foundational Readiness:** Can your data be responsibly shared?
2. **Standardization Readiness:** Can others understand and reuse it?
3. **OMOP Readiness (Optional):** Can it be transformed into a common data model?

You do **not** need to complete every section to begin sharing data. Use what fits your use case/goals.

---

## 🧱 Layer 1: Foundational Data Sharing Readiness

### 🧾 1. Registry Content Inventory

- [ ] **Master variable list** compiled across all data sources  
- [ ] **Data Dictionary** exists for each data set (surveys, labs, genomics, etc.)  
- [ ] **Linkage documentation** describes how sources are joined (e.g., participant ID, visit date)  
- [ ] **Data source tags** included for merged variables (provenance)  
- [ ] **Derived variables** clearly labeled with source(s) documented  
- [ ] **Date standardization** and time alignment addressed  
- [ ] **Missingness summary** reported per source  
- [ ] **Cohort definition** consistent across sources  

---

### 📄 2. Governance & Documentation

- [ ] **Data Use Agreement (DUA)** specifies which data sources are shared  
- [ ] **IRB protocol** covers all data sets and secondary use  
- [ ] **Consent language** reviewed for each source (EHR, biospecimen, survey)  
- [ ] **Oversight committee** includes data set-specific expertise  
- [ ] **Review process** supports partial or multi-source requests  
- [ ] **End-user intake form** asks which data types are requested  
- [ ] **Publications policy** supports tiered or layered access  

---

### 💻 3. Technical Infrastructure

- [ ] **Each data source** available in a common export format (CSV, RDS, JSON, etc.)  
- [ ] **Data integration pipeline** documented (manual or automated)  
- [ ] **De-identified linking key** exists  
- [ ] **Secure transfer options** for large or sensitive files  
- [ ] **Remote analysis environment** available if needed  
- [ ] **Access logs / audit trails** maintained  
- [ ] **Documentation portal or metadata catalog** exists  

---

### 👥 4. Registry Team Roles & Capacity

- [ ] Staff assigned per source (e.g., genomics lead, EHR analyst)  
- [ ] Request fulfillment timelines defined  
- [ ] Capacity to answer provenance and transformation questions  
- [ ] Governance team understands cross-source dependencies  

---

### 🔐 5. Privacy and Ethics

- [ ] **Identifiability risk** assessed across combined data sets  
- [ ] **Omics, imaging, geospatial data** reviewed for re-identification risk  
- [ ] **HIPAA / GDPR compliance** validated per data stream  
- [ ] **Tiered access model** defined (public, controlled, restricted)  
- [ ] **Secure analysis options** offered for sensitive data  
- [ ] **Data destruction policy** covers all formats and systems  

---

## 🧩 Layer 2: Data Standardization Readiness (Recommended)

!!! info "Why is this important?"
    Even well-governed data can be hard to reuse if variables, codes, and meanings are inconsistent.
    This section helps assess **semantic readiness** for harmonization across registries or studies.

---

### 🧠 6. Variable Definitions & Semantics

- [ ] Variables have **clear, unambiguous definitions**  
- [ ] Similar variables across sources are reconciled  
- [ ] Units stored separately and consistently  
- [ ] Dates distinguish **onset vs diagnosis vs observation**  
- [ ] Null values distinguish *missing*, *unknown*, and *not applicable*  

---

### 🧬 7. Standard Vocabulary Use

- [ ] Diagnoses coded or mappable (SNOMED, ORPHA, MONDO)  
- [ ] Phenotypes structured or mappable (HPO)  
- [ ] Labs coded or mappable (LOINC + UCUM units)  
- [ ] Medications normalized (RxNorm / ATC)  
- [ ] Procedures use a recognized coding system  
- [ ] Source values retained alongside standard codes  

---

### 📊 8. Data Quality & Provenance

- [ ] Completeness monitored by source  
- [ ] Value range and format checks defined  
- [ ] Provenance captured for merged variables  
- [ ] data set versions tracked with change logs  

---

## 🧬 Layer 3: OMOP Readiness

!!! note "Optional but Powerful"
    Complete this section if you plan to:
    
      - Participate in federated networks  
      - Enable multi-registry analytics  
      - Support reproducible, model-driven research  

---

### 🧱 9. OMOP Structural Fit

- [ ] Person-level records with stable IDs  
- [ ] Visit or event-based structure  
- [ ] Longitudinal data capture  
- [ ] Core clinical domains represented  

| OMOP Domain | Present |
|------------|---------|
| PERSON | ⬜ |
| VISIT_OCCURRENCE / DETAIL | ⬜ |
| CONDITION_OCCURRENCE | ⬜ |
| MEASUREMENT | ⬜ |
| DRUG_EXPOSURE | ⬜ |
| PROCEDURE_OCCURRENCE | ⬜ |
| OBSERVATION | ⬜ |
| DEATH | ⬜ |

---

### 🔄 10. OMOP ETL Practicality

- [ ] Source tables are stable  
- [ ] Variable meanings are consistent  
- [ ] Units explicitly stored  
- [ ] Dates are parseable and complete  
- [ ] Corrections and updates can be tracked  

---

### 📐 OMOP Readiness Scale & Rubric

!!! tip "What This Scale Is For"
    This rubric helps registries understand **how close they are to OMOP Common Data Model (CDM) adoption**, and what steps are needed to move forward.

    OMOP readiness is **not all-or-nothing.** Many registries progress through these levels over time.

---

#### 🚦 OMOP Readiness Levels (0–4)

##### **Level 0: Not OMOP-Ready**
**Status:** Foundational gaps prevent OMOP mapping.

**Typical characteristics**
- No stable person identifiers  
- Flat or cross-sectional data only  
- Heavy reliance on free text for key domains  
- No consistent visit or event dates  
- Variable definitions unclear or missing  

**What to focus on next**
- Create a master data dictionary  
- Define person- and event-level structure  
- Standardize dates, identifiers, and provenance  

---

##### **Level 1: Structurally Aware**
**Status:** Data structure exists, but semantics are weak.

**Typical characteristics**
- Person-level records with stable IDs  
- Longitudinal data present  
- Minimal or inconsistent use of standard vocabularies  
- Local codes or free text dominate  
- Mapping would rely heavily on OMOP `OBSERVATION`  

**What to focus on next**
- Clarify variable definitions  
- Identify candidate standard vocabularies  
- Normalize units and dates  

---

##### **Level 2: Terminology Mappable**
**Status:** Core domains can be mapped with moderate effort.

**Typical characteristics**
- Diagnoses, labs, and medications partially coded or mappable  
- Units stored separately  
- Source values preserved  
- Visit structure mostly consistent  
- Limited governance around vocabularies  

**What to focus on next**
- Formalize vocabulary mappings  
- Reduce free text in high-value fields  
- Document mapping decisions  

---

##### **Level 3: OMOP-Compatible**
**Status:** OMOP ETL feasible with standard effort.

**Typical characteristics**
- Core clinical domains map cleanly to OMOP tables  
- Standard vocabularies used consistently  
- Longitudinal visits or events well-defined  
- Provenance and versioning tracked  
- Initial OMOP ETL completed or piloted  

**What to focus on next**
- Expand to additional domains (e.g., genomics, PROs)  
- Improve automation and quality assurance  
- Prepare for federated analyses  

---

##### **Level 4: OMOP-Operational**
**Status:** OMOP is production-ready and reusable.

**Typical characteristics**
- Routine OMOP refreshes  
- Automated and versioned ETL pipeline  
- Data quality checks aligned with OMOP conventions  
- Participation in federated or networked studies  
- Clear governance for mappings and updates  

**What to focus on next**
- Optimization and performance  
- Advanced phenotyping and cohort reuse  
- Cross-network harmonization  

---

#### 📊 How to Assign a Level

Use the OMOP checklists above and apply the following rule:

- **Level 0:** Fails multiple Structural Fit items  
- **Level 1:** Structural Fit ✔, Terminology Mapping mostly ✖  
- **Level 2:** Structural Fit ✔, Terminology Mapping mostly ✔  
- **Level 3:** Structural + Terminology + ETL Practicality ✔  
- **Level 4:** Level 3 plus operationalized ETL and reuse  

---

#### 🧮 Optional Quantitative Scoring

Assign points to each OMOP readiness checklist item:

- ✔ = 1 point  
- ✖ = 0 points  

**Score ranges**
- **0–4:** Level 0  
- **5–8:** Level 1  
- **9–12:** Level 2  
- **13–16:** Level 3  
- **17+**: Level 4  

---

## 🧩 Tips for Multi-Source Registries

- Use **data source tagging** and consistent naming conventions  
- Track **data provenance**: what came from where, and when  
- Clarify which data sources are **required vs optional**  
- Share **core data sets by default**, restrict sensitive or high-dimensional data  
- Provide diagrams of **data architecture or flow**  

---

## 📌 Summary

Use this assessment to identify gaps **before** inviting data access requests or pursuing harmonization.

Many registries begin with Layer 1, progress through Layer 2, and only complete Layer 3 when needed.

Consider publishing a **data inventory table** summarizing each source, access level, and documentation status.

---

*Need help? Visit the [How to Customize This Template](customization.md) page or contact your data governance advisor.*

