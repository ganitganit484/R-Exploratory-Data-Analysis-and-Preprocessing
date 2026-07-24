# R-Exploratory-Data-Analysis-and-Preprocessing
# Data Analysis & Preprocessing in R (Admissions & Titanic)

This repository contains an exploratory data analysis (EDA) and data cleaning project written in R using `dplyr` and `ggplot2`. 

The project focuses on practical data preprocessing (handling missing values with statistical justifications) and uncovering relationships across two different datasets.

## Project Structure

### 1. Graduate Admissions Analysis
Analyzing applicant characteristics and their impact on Master's program admission chances.
* **Missing Data Strategy:** Imputed missing `GRE` scores using the median to avoid outlier bias, and `CGPA` using the mean due to its symmetric distribution.
* **Key Findings:**
  * Applicants with research experience had a noticeably higher average CGPA (8.89 vs. 8.26).
  * A clear positive trend exists between University Rating and applicant TOEFL scores (averaging 99.1 in Rating 1 up to 114.0 in Rating 5).

### 2. Titanic Survival Analysis
Investigating socio-economic and demographic factors affecting passenger survival.
* **Missing Data Strategy:** Missing `Age` values were imputed with group medians, `Cabin` missingness was assigned as `"Unknown"`, and missing `Embarked` ports were filled with the mode (`"S"`).
* **Key Findings:**
  * **Class & Gender:** 1st-class females had a 96.3% survival rate, compared to just 15.2% for 3rd-class males.
  * **Child Survival Gap:** 100% of 2nd-class children survived, whereas 3rd-class children had a 47.4% survival rate.
  * **Family Size Effect:** Passengers traveling with larger families (>2 siblings/spouses) were almost strictly in 3rd class, suffering lower survival rates due to both economic location and evacuation logistics.

## Tech Stack & Packages
* **Language:** R
* **Libraries:** `dplyr`, `ggplot2`, `tidyr`, `knitr`

## Repository Files
* `Assignment.Rmd` - Source RMarkdown code and commentary.
* `Assignment.html` - Knitted report with generated plots and formatted tables.
