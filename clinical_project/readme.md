# **Clinical Dataset**

## **Overview**

This project analyzes 2 clinical datasets, a discovery cohort and a validation cohort  using Python to uncover relationships between cancer stage and death events and other factors including sex, smoking, gene mutation presence, etc.

The goal is to demonstrate data cleaning, exploratory data analysis (EDA), and data visualization skills using Python.

## **Objective**

This project answers the following questions:

* How many female patients vs male patients?  
* Which stages had the highest mortality rates?  
* Is there any correlation between tumor size or smoking and survival time?  
* Does gene mutation affect survival time?

## **Dataset**

Source: Clinical Dataset (Kaggle)

The dataset contains information, including:

Discovery cohort:

* id  
* Specimen date  
* Dead or alive  
* Date of death  
* Date of last follow up  
* Sex  
* Race  
* Stage  
* Event  
* time

Validation cohort:

* Id  
* Survival time (days)  
* event\_(death:\_1,\_alive:\_0)  
* Tumor size in cm  
* Grade  
* Stage (tnm 8th edition)  
* Age  
* Sex  
* Cigarette  
* Pack per year  
* Type adjuvant  
* Batch  
* EGFR  
* KRAS

## **Tools and Libraries**

* Python  
* Pandas  
* Matplotlib  
* Seaborn  
* Jupyter Notebook

## **Project Workflow**

### **1\. Data Cleaning**

* Handled missing values  
* Standardized column formats  
* Converted date fields to appropriate data types  
* Fixing text mistakes.

### **2\. Exploratory Data Analysis**

* Analyzed the distribution of categorical variables such as sex, race, and people who used cigarettes using countplots.   
* Analyzing relationships between variables through scatter plots. 

### **3\. Data Visualization**

Created visualizations including:

* Count plots  
* Bar charts  
* Scatter plots

## **Key Findings**

Discovery cohort:

* The records of this cohort showed that most patients were deceased.  
* Number of patients was almost the same, with slightly more males than females.  
* Most patients in this cohort were white, with way less black patients, and even less patients whom were asian or from other races.  
* The highest number of deaths was observed in patients who were diagnosed with T1N0 stage, with 7 deaths out of 9 patients, followed by T2N0 stage with 5 deaths out of 11 patients.  
* The percentage of deaths amongst males was higher than that of females.  
* Percentage of deaths amongst black patients was higher than that of white patients.

Validation cohort:

* More female patients were in the cohort than men, almost the double.  
* The percentage of deaths amongst males was higher than that of females.  
* Most patients were former smokers, some of them never smoked and a smaller number of them were current smokers.  
* Most cases showed negative results for EGFR and KRAS mutations  
* No correlation observed between tumor size and survival time.  
* No correlation observed between cigarette packs number per year and survival time  
* Most deaths were observed in the IIIA stage, followed by IA2, IB, IIB stages.  
* Most deaths were also observed in the third grade followed by the second grade then the first with the least number of deaths. 

## **Limitations**

The discovery and validation cohorts used different clinical variables, limiting direct comparison between datasets.

The cancer type was not specified in the dataset documentation, limiting the clinical interpretation of findings.

This project focused on exploratory data analysis and descriptive statistics; therefore, no causal relationships or clinical conclusions can be inferred from the results.