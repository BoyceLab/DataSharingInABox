# Choosing a Secure Storage Platform for Shared Registry Data

Patient registry teams must carefully consider where and how to store and share data, particularly when sharing with external researchers. The platform used should support regulatory compliance, data privacy, secure access, scalability, and usability across technical skill levels. Below is a breakdown of key storage and access models, major cloud vendors, and important considerations for implementation.

## 🔐 Data Hosting Options

### 1. Cloud-Based Platforms

- **Amazon Web Services (AWS)**
  - HIPAA-eligible services (e.g., S3, RDS, EC2)
  - Supports secure data lakes, analytics, and machine learning
  - Common choice for enterprise health data infrastructure
  - Broad integration with Python/R/SQL-based notebooks (e.g., SageMaker, EMR)

- **Microsoft Azure**
  - Trusted by many academic medical centers
  - Tools for AI/ML, relational databases, and Azure Synapse Analytics
  - Provides granular identity and access control

- **Google Cloud Platform (GCP)**
  - Popular in research computing (BigQuery, Cloud Datalab)
  - Optimized for analytics-heavy workflows
  - Strong support for FHIR and healthcare APIs

### 2. Local/Institutional Servers

- Maintained by your own organization (e.g., hospital IT, university research computing)
- May be required by data governance agreements
- Pros: direct control, no third-party exposure
- Cons: scaling, security patching, and external access can be more difficult

---

## 🔍 Key Questions to Ask

- Does the platform meet **HIPAA**, **GDPR**, or **IRB** requirements?
- What data access controls are supported (e.g., single sign-on, user audit logs)?
- Are there approved environments for **PHI** or limited data sets?
- What types of users will need access (e.g., R users, Python users, Stata/SPSS users)?
- Will external collaborators work within a **secure enclave** or receive downloaded datasets?

---

## 💡 Enclave Environments: An Alternative to Downloading Data

Instead of providing datasets for download, some registries use a **secure enclave**—a virtual environment where researchers log in to conduct analyses remotely. These setups often use Jupyter Notebooks, RStudio Server, or even locked-down terminal access. 

### Benefits
- Enhanced security: no raw data leaves the enclave
- Audit logs and reproducibility
- Easier to control software, packages, and compute environments

### Limitations and Considerations
- Users must adapt to cloud-based workflows (e.g., notebooks)
- Some researchers prefer point-and-click tools (e.g., SPSS/Stata)
- Requires robust user support and onboarding
- Data visualization may be limited unless tools are configured

### Examples of Enclave Tools
- AWS SageMaker Studio Lab / EC2 JupyterHub
- Microsoft Azure Machine Learning Workspaces
- GCP Vertex AI Workbench
- NIH's BioData Catalyst / dbGaP Authorized Access Workspaces

---

## 🔄 Summary: Match Tools to Users
| Feature/Need                  | Best Fit Platform       |
|------------------------------|--------------------------|
| Raw statistical file sharing | Encrypted cloud folder or secure FTP |
| SQL analysis and reporting   | Cloud-hosted RDS or BigQuery |
| Notebook-based collaboration | AWS/GCP/Azure Notebooks or JupyterHub |
| Protected health information | Enclave with IRB + DUA controls |

When in doubt, start with a small pilot and gather user feedback before expanding access.

---

For policy implications and best practices, see the [NIH Data Sharing Language Explained](nih-data-sharing.md) section.

