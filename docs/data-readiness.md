# ✅ Data Sharing Readiness Assessment

!!! warning "Disclaimer"
    This is **sample content only**. It is intended as a general framework for registry holders or patient advocacy groups to evaluate data sharing readiness.  
    Please consult your legal, IRB, or data governance advisors before using this tool in a live environment.

!!! tip "Purpose of This Checklist"
    This page helps registry holders or patient advocacy groups assess their **data sharing readiness** by reviewing data assets, documentation, infrastructure, and governance practices.  
    It is especially useful if your registry includes **multiple data sources** (e.g., EHR, surveys, biosamples, imaging, omics).
---

## 🧾 1. Registry Content Inventory

- [ ] **Master variable list** compiled across all data sources  
- [ ] **Data Dictionary** exists for each dataset (surveys, labs, genomics, etc.)  
- [ ] **Linkage documentation** describes how sources are joined (e.g., participant ID, visit date)  
- [ ] **Data source tags** are included for merged variables (to show provenance)  
- [ ] **Derived variables** are well-labeled and their source(s) are documented  
- [ ] **Date standardization** and time alignment across sources is addressed  
- [ ] **Missingness summary** reported per source  
- [ ] **Cohort definition** is consistent across sources (e.g., same inclusion/exclusion)

---

## 📄 2. Governance & Documentation

- [ ] **Data Use Agreement (DUA)** specifies which data sources are shared  
- [ ] **IRB protocol** covers all datasets and secondary use  
- [ ] **Consent language** reviewed for each source (e.g., biospecimen, EHR, survey)  
- [ ] **Oversight committee** includes representation familiar with each dataset type  
- [ ] **Review process** handles requests for partial or multi-source data  
- [ ] **End-user survey or intake form** asks which data types are needed  
- [ ] **Publications policy** considers layered or tiered access (e.g., core data vs. omics)

---

## 💻 3. Technical Infrastructure

- [ ] **Each data source** is available in a common export format (CSV, RDS, JSON, etc.)  
- [ ] **Data integration pipeline** (manual or automated) is described  
- [ ] **De-identified linking key** exists to join data while protecting identity  
- [ ] **Secure transfer options** accommodate large files (e.g., genomics, imaging)  
- [ ] **Remote analysis environment** is available for high-sensitivity data  
- [ ] **Access logs or audit trails** are maintained per data source  
- [ ] **Documentation portal** or metadata catalog exists per dataset

---

## 👥 4. Registry Team Roles & Capacity

- [ ] Staff assigned to curate and support each source (e.g., genomics lead, EHR analyst)  
- [ ] Request fulfillment timelines defined based on source complexity  
- [ ] Capacity exists to answer data provenance and transformation questions  
- [ ] Governance team understands dependencies between sources

---

## 🔐 5. Privacy and Ethics

- [ ] **Identifiability risk** assessed across combined datasets  
- [ ] **Omics, imaging, and geospatial data** are reviewed for re-ID risk  
- [ ] **HIPAA / GDPR-compliance** validated per data stream  
- [ ] **Tiered access models** considered (e.g., public, controlled, restricted)  
- [ ] **Secure analysis environments** offered for sensitive linked datasets  
- [ ] **Data destruction policy** covers all file types and storage methods

---

## 🧩 Tips for Multi-Source Registries

- Use **data source tagging** and clear naming conventions in merged files.  
- Track **data provenance**: what came from where, and when.  
- Clearly indicate whether all sources are required for analysis, or optional.  
- Consider **sharing core datasets by default**, and requiring justification for sensitive or high-dimensional data (e.g., omics).  
- Provide visual diagrams of the **data architecture or flow**, especially if complexity is high.

---

## 📌 Summary

Use this checklist to identify gaps before inviting data access requests — especially when managing diverse or sensitive datasets.  
Consider publishing a **data inventory table** summarizing each source, its variables, access level, and documentation status.

---

*Need help? Visit the [How to Customize This Template](customization.md) page or contact your data governance advisor.*
