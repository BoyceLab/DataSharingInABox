# Guidance for Sharing Patient Tracker or Registry Data with Clinical Trial Sponsors
---

!!! note "Disclaimer"
    This document provides general guidance and is not legal advice.  
    Legal, regulatory, and ethics experts should be consulted before implementing data-sharing practices.

---
## 1. Purpose

This document establishes a policy for the responsible sharing of **patient-generated data (PGD)** collected through a patient advocacy group's tracker application or patient registry. It is intended to protect:

- Clinical trial integrity
- Patient privacy and informed consent
- Ethical and regulatory compliance
- Scientific credibility

---

## 2. Scope

This policy applies to:

- A symptom tracker app or registry operated by the advocacy group
- Any biopharmaceutical company (“Sponsor”), including those:
  - Conducting ongoing clinical trials
  - Planning future trials

It governs sharing of:

- Aggregate and individual-level data
- Historical and contemporaneous datasets
- Scientific, commercial, and regulatory uses of patient-generated data

---

## 3. Regulatory Background: Key Quotes

### 3.1 FDA Guidance on RWD/RWE (2021)

> “FDA emphasizes the importance of **prospective planning** of data sources, data management procedures, and analytic methods… Deviations from prespecified plans may undermine the reliability of the evidence.”

Source: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/considerations-use-real-world-data-and-real-world-evidence-support-regulatory-decision-making-drug

> “If data originate outside of the clinical trial data collection system, sponsors should ensure the data **cannot bias** or otherwise influence the conduct or interpretation of the trial.”

---

### 3.2 FDA Draft Guidance on Blinding in Clinical Trials (2024)

> “Access to information that could reveal or suggest treatment assignment must be controlled. Sponsors should ensure that personnel involved in trial conduct or interpretation do **not have access to data streams that could introduce bias**.”

Source: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/blinding-clinical-trials

> “External sources of information may provide unintended unblinding.”

---

### 3.3 FDA Guidance: Assessing Registries for Regulatory Use (2023)

> “To be suitable for regulatory use, the data elements, data capture processes, and analyses should be **prespecified**.”

Source: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/real-world-data-assessing-registries-support-regulatory-decision-making-drug-and-biological-products

> “Unplanned analyses of RWD may introduce bias.”

---

### 3.4 EMA Guideline on Computerised Systems in Clinical Trials (2023)

> “All data used in clinical trials must be **prospectively defined**, captured, processed, and stored in validated systems under the control of the sponsor or investigator.”

Source: https://www.ema.europa.eu/en/documents/regulatory-procedural-guideline/guideline-computerised-systems-and-electronic-data-clinical-trials_en.pdf

> “Uncontrolled or unsupervised data sources risk compromising data integrity, auditability, and trial reliability.”

---

### 3.5 EMA Reflection Paper on External Controls and RWD

> “The use of external data must be supported by **prospective planning**, robust governance, and documented quality controls.”

Source: https://www.ema.europa.eu/en/development-reflection-paper-use-external-controls-evidence-generation-regulatory-decision-making-scientific-guideline

> “Pre-specification of data sources and analytic rules is essential to avoid operational and analytical bias.”

---

### 3.6 ICH E6(R3) Good Clinical Practice Draft

> “The protocol should describe **all planned data sources**, data collection methods, and procedures to assure data quality.”

Source: https://www.ich.org/page/efficacy-guidelines

> “Processes should ensure that trial personnel remain free from information that could unduly influence trial conduct or interpretation.”

---

## 4. Key Principles

### 4.1 Prospective Planning

All data sources and intended uses must be predefined. Non-prospectively planned data sharing is discouraged.

### 4.2 Protection of Clinical Trial Integrity

PGD must not:

- Unblind or risk unblinding
- Provide informal interim signals
- Influence trial conduct
- Circumvent DSMB/IDMC processes

### 4.3 Consent & Privacy

- Sharing must align with the tracker app’s consent
- De-identification must meet relevant regulatory standards
- Re-identification risk must be assessed

### 4.4 Data Governance

Requires:

- A Data Use Agreement (DUA)
- Documented sponsor firewalls

### 4.5 Transparency

Patients should understand potential data-sharing practices.

---

## 5. When Data Sharing Is Permissible

### 5.1 De-Identified or Anonymized Data

- Meets HIPAA/GDPR standards
- Re-identification risk assessed

### 5.2 Limited Impact on Trials

- Historical (non-contemporaneous)
- Aggregated
- Cannot reveal efficacy or safety trends

### 5.3 Governance and Firewalls

- DUA in place
- Access limited to RWE teams
- Trial teams excluded

### 5.4 Clear, Pre-Specified Use

Examples:

- Natural history studies
- Burden-of-illness projects
- HEOR
- Non-regulatory scientific uses

### 5.5 Ethics Oversight

Recommended for small rare-disease populations.

---

## 6. When Data Sharing Is Not Permissible

High-risk scenarios:

- Contemporaneous patient-level symptom data
- Data revealing efficacy/safety trends
- Likely overlap with trial participants
- Inadequate consent
- No DUA or governance
- Ad hoc exploratory sponsor requests
- Any sharing that could bias trial conduct

**Important:** The issue exists even if the sponsor does **not** intend to use the data in a regulatory submission. Regulators assess whether access *could have influenced* the trial.

---

## 7. Operational Safeguards

### 7.1 Data Preparation

- Predetermined data fields
- De-identified
- Aggregated

### 7.2 Timing Controls

- Lag of ≥3–6 months
- Avoid sharing during blinded phases

### 7.3 Sponsor Firewalls

Allowed:

- RWE / Epidemiology
- HEOR
- Privacy/security teams

Prohibited:

- Clinical operations
- Trial statisticians
- Medical monitors
- Protocol authors

### 7.4 Auditability

- Logs of all transfers
- Access logs inside sponsor systems
- Annual review

---

## 8. Roles and Responsibilities

### Advocacy Group / Data Controller

- Consent management
- De-identification
- Risk assessments
- DUA enforcement

### Sponsor

- Maintain firewalls
- Control internal access
- Avoid trial contamination

### Oversight Committee (Optional)

- Review high-risk cases
- Advise on ethics and expectations

---

## 9. Data-Sharing Checklist

### Purpose

- [ ] Purpose defined
- [ ] Sponsor trial activity identified
- [ ] Regulatory vs non-regulatory use clarified

### Data Characteristics

- [ ] Type
- [ ] Aggregation level
- [ ] Timing
- [ ] Granularity

### Consent & Privacy

- [ ] App consent allows sharing
- [ ] Re-identification risk reviewed
- [ ] HIPAA/GDPR compliance documented

### Trial Integrity

- [ ] Overlap with trial evaluated
- [ ] Unblinding risk assessed
- [ ] Firewall documented

### Governance

- [ ] DUA signed
- [ ] Named data recipients
- [ ] Prohibited teams identified
- [ ] Access controls set
- [ ] Logs enabled

### Risk Rating

- [ ] Green: acceptable
- [ ] Amber: acceptable with safeguards
- [ ] Red: not permissible

---

## 10. Safe Sharing Model (Table Format)

### Data Flow Overview

| Step | Description | Flow |
|------|-------------|------|
| 1 | PGD collected | App → Advocacy Group |
| 2 | De-identified + aggregated | Advocacy Group → Prepared Dataset |
| 3 | Shared only with RWE | Prepared Dataset → Sponsor RWE Team |
| 4 | Firewalls enforced | RWE Team → (No access to Trial Team) |
| 5 | Optional high-level insights | RWE Team → Filtered Summary → Trial Team (optional) |

### Sponsor Access Rules

| Team | Access to PGD | Notes |
|------|----------------|-------|
| RWE / Epidemiology | Yes | Primary recipients |
| HEOR | Yes | Aggregate use only |
| Privacy/Security | Yes | Compliance only |
| Clinical Operations | No | Firewalled |
| Trial Statisticians | No | Firewalled |
| Medical Monitors | No | Firewalled |
| Protocol Authors | No | Firewalled |

---


