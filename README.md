## OAI Dataset Analysis: In-Depth Exploration of Osteoarthritis Progression and Risk Factors

This project provides a detailed, step-by-step analysis of the Osteoarthritis Initiative (OAI) dataset, designed to uncover key insights into osteoarthritis (OA) progression and associated risk factors. Through comprehensive data processing, visualization techniques, and rigorous statistical testing, this project aims to deepen understanding of OA and its demographic variances.

**Project Overview:**

This repository delivers a robust analytical framework for researchers and data enthusiasts seeking to explore the complexities of osteoarthritis using the OAI dataset. The project systematically progresses from raw data to actionable insights through distinct stages:

*   **Data Harmonization**: We begin by accessing and integrating diverse datasets from the OAI, including participant demographics, clinical measurements, and radiographic assessments (KL grades).
*   **Exploratory Data Analysis (EDA)**:  Utilizing powerful Python libraries such as Pandas, Matplotlib, and Seaborn, we perform comprehensive data cleaning, preprocessing, and feature engineering to prepare the dataset for analysis.
*   **Visual Analytics**: We generate a range of visualizations, including distribution plots, comparative box plots, and longitudinal trend lines to effectively explore patterns, anomalies, and relationships within the data.
*   **Statistical Hypothesis Testing**: We implement advanced statistical methods, specifically bootstrapping, to conduct two-sample tests and estimate confidence intervals, allowing for rigorous assessment of hypotheses regarding differences in OA prevalence across demographic groups.

**Project Stages:**

*   **Stage 1: OAI Data Access and Environment Setup**
    *   Guides users through the necessary steps to request and gain access to the OAI dataset from the NIH Data Archive, emphasizing ethical and legal data handling.
    *   Sets up the Python environment with required libraries, ensuring reproducibility and ease of use.

*   **Stage 2: Data Loading, Processing, and Integration**
    *   Implements robust data loading pipelines to read various OAI data files (`.txt` format) into Pandas DataFrames.
    *   Executes comprehensive data cleaning and preprocessing steps, including handling missing values and data type conversions.
    *   Merges demographic, clinical, and KL-grade datasets into unified longitudinal dataframes using Pandas' powerful merging capabilities, facilitating patient-centric analysis across multiple visits.

*   **Stage 3: Exploratory Data Analysis and Visualization**
    *   Generates insightful visualizations to understand data distributions and relationships:
        *   Bar charts for participant counts across different acquisition sites.
        *   Box plots illustrating the relationship between BMI and KL grades at baseline.
        *   Line plots showing trends of KL grade progression over time for different acquisition sites, incorporating confidence intervals for statistical reliability.

*   **Stage 4: Statistical Hypothesis Testing via Bootstrapping**
    *   Applies bootstrapping techniques for rigorous statistical analysis:
        *   Implements bootstrap resampling to generate distributions of test statistics, enabling non-parametric inference.
        *   Calculates both naïve percentile and refined normal distribution confidence intervals to quantify uncertainty and estimate true metric ranges.
        *   Performs two-sample hypothesis testing to investigate significant differences in KL grades between gender groups within a specific age cohort (age >= 60).
        *   Computes and interprets two-sided p-values to make statistically sound conclusions about the null hypothesis of no difference between groups.

**Key Analyses and Implementations:**

*   **Demographic Analysis**:
    *   Counts and visualizes participant distribution by sex and acquisition site, revealing cohort composition and potential site-specific biases.

*   **BMI and Baseline OA Severity**:
    *   Analyzes and visualizes the association between Body Mass Index (BMI) and Kellgren-Lawrence (KL) grades at the baseline visit, exploring baseline risk factors.

*   **Longitudinal KL Grade Trend Analysis**:
    *   Visualizes the progression of KL grades over up to 96 months of follow-up, segmented by acquisition site, highlighting potential site-specific disease trajectories and variations.
    *   Incorporates 95% confidence intervals in trend visualizations to provide a measure of the statistical certainty of observed trends.

*   **Two-Sample Hypothesis Testing via Bootstrapping**:
    *   Employs bootstrapping for non-parametric hypothesis testing to compare KL grades between elderly men and women (age >= 60).
    *   Calculates and interprets p-values to determine if observed differences are statistically significant, assessing gender-based disparities in OA severity within the older demographic.
    *   Estimates 95% confidence intervals using both naïve percentile and normal distribution methods to quantify the range and uncertainty of observed KL grade differences.

**Dataset Access:**

The code in this repository is designed to process and analyze data from the Osteoarthritis Initiative (OAI) dataset. **Please note that the full OAI dataset is not publicly available for direct download due to data usage agreements.**

To access and utilize the full dataset, you will need to apply for access through the NIH (National Institutes of Health) Data Archive (NDA).  Please follow these general steps:

1.  Visit the [NIH Data Archive (NDA) website](https://nda.nih.gov/) or the [Osteoarthritis Initiative (OAI) homepage](https://nda.nih.gov/oai/).
2.  Register for an NDA account if you do not already have one.
3.  Search for the "Osteoarthritis Initiative (OAI)" dataset within the NDA.
4.  Follow the NDA's instructions to request access. This typically involves agreeing to a Data Use Certification/Agreement and may require a brief description of your research purpose.

**For more specific instructions or to start your application, please refer to the OAI section of the NDA website or consult the documentation provided with the OAI dataset itself once you have access.**

Once you have been granted access and have downloaded the data files, ensure you place the `OAICompleteData_ASCII` folder (or the data files you downloaded) in the same directory as the notebook to run the code correctly.

**Libraries Used:**

*   Python (>=3.9)
*   Pandas (>=1.5)
*   NumPy (>=1.23)
*   Matplotlib (>=3.6)
*   Seaborn (>=0.12)
*   Pathlib (standard Python library)

**Author:** Ata Jodeiri Seyedian
**Emails:** ata.jodeiri@student.oulu.fi, sataseyedian@gmail.com
