---
title: Data Sharing Readiness Assessment
toc: true
---

## ✅ Data Sharing Readiness Assessment

!!! tip "Purpose of This Checklist"
    This page helps registry holders, patient advocacy groups, and data stewards assess their **data sharing readiness**  including documentation, governance, technical infrastructure, and **data standardization**.

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

### 🚦 OMOP Readiness Rating

- **Green** – OMOP ETL feasible now  
- **Yellow** – Standardization needed first  
- **Red** – Not currently suitable  

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
