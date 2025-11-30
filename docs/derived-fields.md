!!! warning "Sample Content Only"
    This page contains **example language and placeholders** designed to help registry teams build their own data sharing site.  
    Please **replace all placeholder text** with details specific to your own project, policies, and governance requirements.
    
# Derived Fields Documentation

*This page explains any derived or calculated fields in the registry dataset.* Derived fields are those not collected directly, but computed from other data. Documenting them is important for transparency and reproducibility.

For each derived variable, explain how it’s calculated or defined. For example:

- **Body Mass Index (BMI):** Calculated as weight (kg) divided by squared height (m^2), using the most recent weight and height from the patient record.
- **Age Group:** Derived from the exact age; categorized into groups (0-17 = child, 18-64 = adult, 65+ = senior) at time of enrollment.
- **Disease Duration:** Computed as the time in years from reported diagnosis date to the last follow-up date.

*Instructions:* Replace the examples with your actual derived fields. Provide enough detail that another researcher could recreate the field from the source data. If a derived field comes from an external algorithm or reference, cite or describe that as well.
