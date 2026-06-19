# Project: AI Dependency, Career Anxiety, and Student Burnout Analysis

This repository contains a foundational data analytics workflow utilizing **Python**, **Pandas**, and **Matplotlib/Seaborn** to analyze student survey data regarding AI's impact on career anxiety.

---

##  Analytics Workflow & Methodology

### 1. Data Acquisition
* **Source:** Kaggle Dataset – [AI Dependency, Career Anxiety, and Student Burnout](https://www.kaggle.com/datasets/sridipbasu/ai-depndency-career-anxiety-and-student-burnout)
* **File Analyzed:** `ai_dependency_career_anxiety_students.csv`

### 2. Data Cleaning & Preprocessing
* **Handling Missing Values:** Identified approximately 1,000 to 1,500 null values across 3–4 specific features.
* **Action:** Executed listwise deletion (`df.dropna()`) across these columns to ensure statistical validity and prevent skewing downstream visualizations.

### 3. Exploratory Data Analysis (EDA)
Initial structural and statistical profiling was conducted using standard Pandas validation methods:
* `df.info()`: Evaluated structural data types, memory usage, and non-null counts.
* `df.describe()`: Generated descriptive statistics (mean, median, standard deviation, quartiles) for numeric attributes.
* `df.head()` & `df.sample()`: Inspected raw records to map categorical distributions and structural formatting.

### 4. Demographic & Cohort Segmentation (Visualizations)

#### A. Global Student Population Gender Ratio
* **Visualizations:** Comparative Analysis using **Pie Charts** and **Bar Charts**.
* **Technical Implementation:** Configured dynamic percentages via `autopct='%1.1f%%'` and optimized color palettes for high-contrast readability.

#### B. Engineering Cohort (CSE/IT Stream)
* **Methodology:** Filtered data to isolate students enrolled explicitly in Computer Science and Information Technology pathways.
* **Analysis:** Extracted and visualized the localized gender distribution within this tech-focused demographic.

#### C. Management Cohort (MBA Degree)
* **Methodology:** Isolated records corresponding to Master of Business Administration (MBA) candidates.
* **Analysis:** Conducted a comparative gender ratio analysis against the global and engineering baselines.

---

##  Technology Stack
* **Language:** Python 3.x
* **Environment:** Jupyter Notebook
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
