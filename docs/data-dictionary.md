!!! warning "Sample Content Only"
    This page contains **example language and placeholders** designed to help registry teams build their own data sharing site.  
    Please **replace all placeholder text** with details specific to your own project, policies, and governance requirements.
    
# Data Dictionary

*This page provides a detailed data dictionary for the registry.* Below is a list of the key data fields collected, along with their definitions and allowable values. Use this as a reference to understand the data set.

<!-- Example structure: you might use a table or list to present the data dictionary. Here's a suggestion for a table format: -->

| **Field Name**       | **Description**                                | **Type / Units**        | **Notes**                           |
| -------------------- | ---------------------------------------------- | ----------------------- | ----------------------------------- |
| `patient_id`         | Unique identifier for each patient             | Integer                 | (e.g., study ID, no personal info)  |
| `enrollment_date`    | Date the patient was enrolled in the registry  | Date (YYYY-MM-DD)       |                                    |
| `age_at_enrollment`  | Age of patient at time of enrollment           | Integer (years)         | Derived from DOB and enrollment date|
| *...add your fields...* |                                            |                         |                                     |

*Instructions:* Edit the table above to include **all variables** in your data set. For each field, provide a clear description. Include units or format (e.g., "Date (YYYY-MM-DD)" or "Categorical: 0=No, 1=Yes"), and any notes (like derivation or if the field is optional). If your registry has multiple tables or modules of data, you could split this into multiple pages or sections.
