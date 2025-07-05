# Google-Health-AI-Hackaton
Repo for Google Health AI Hackaton (Paris, 05/07/2025)

**Project Overview**
Our team set out to solve a recurring in healthcare: errors in clinical data. Drawing from real-world experience at Orakl Oncology, a techbio startup, we’ve seen how data quality issues like timeline inconsistencies or misclassified treatments can derail months of research. At Orakl, cleaning a single dataset could take 3 to 4 months and significantly delayed model deployment. After cleaning, performance improved by 10%, confirming the huge impact of data quality.

These issues are not unique to us. Clinical data is often manually entered by clinicians or transcribed from old paper records, introducing significant noise. According to literature, error rates reach an average of 976 errors per 10,000 fields in source-to-database audits (PLOS ONE).
https://www.sciencedirect.com/science/article/pii/S1556086415320761

**Our Solution**
To address this, we built a pipeline based on MedGemma, the multimodal model from Google optimized for medical data. Our system allows a data scientist to upload a cohort table and, through several calls to MedGemma, automatically produces a structured error report. It transforms raw, messy tables into actionable quality insights—without needing weeks of manual review.

**Methodology**
To evaluate the system’s effectiveness, we created a synthetic dataset inspired by Orakl data from the Gustave Roussy Institute (anonymized). We methodically introduced different types of known errors based on our domain experience:<br>
-Timeline inconsistencies<br>
-Contradictory diagnoses<br>
-Implausible treatment outcomes<br>
-Missing values or corrupted entries<br>

This allowed us to benchmark our tool’s performance in detecting clinically meaningful issues.

**Impact**
This tool can help pharmaceutical companies, biotech startups, and research labs restore trust in their data, reduce manual review time, and accelerate discovery. By automating one of the most painful parts of the clinical AI pipeline, we aim to unlock faster and more reliable insights from clinical datasets.


![Diagram](https://github.com/tarantop/Google-Health-AI-Hackaton/blob/main/Google%20Hackathon.png?raw=true)
