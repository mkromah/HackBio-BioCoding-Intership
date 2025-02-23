# **HackBio Internship – BioCoding Series**

## **📌 Table of Contents**
1. [Introduction](#introduction)
2. [Team Information](#team-information)
3. [Task 0: Team Formation & Data Representation](#task-0-team-formation--data-representation)
4. [Task 1: Microbial Growth Curve Analysis](#task-1-microbial-growth-curve-analysis)
5. [Task 2: Advanced Bioinformatics Analyses](#task-2-advanced-bioinformatics-analyses)
   - [2.1 Microbiology: Growth Curve Analysis](#21-microbiology-growth-curve-analysis)
   - [2.3 Botany & Plant Science: Metabolic Response Analysis](#23-botany--plant-science-metabolic-response-analysis)
   - [2.4 Biochemistry & Oncology: Protein Mutation Impact](#24-biochemistry--oncology-protein-mutation-impact)
   - [2.6 Transcriptomics: RNA-seq Data Analysis](#26-transcriptomics-rna-seq-data-analysis)
   - [2.7 Public Health: NHANES Data Analysis](#27-public-health-nhanes-data-analysis)
6. [Upcoming Tasks](#upcoming-tasks)
7. [How to Contribute](#how-to-contribute)
8. [Contact & Socials](#contact--socials)

---

## **Introduction**
This repository documents the **HackBio BioCoding Internship**, where we engage in bioinformatics problem-solving using **Python and R**. Our goal is to enhance our coding proficiency while applying computational techniques to biological datasets.

---

## **Team Information**
| Name                     | Slack Username | Email                      | Hobby               | Country  | Discipline       | Preferred Language |
|--------------------------|---------------|----------------------------|----------------------|----------|-----------------|--------------------|
| Musa Al Hassan Kromah    | Musa          | kromahmusa86@gmail.com     | Hiking              | Liberia  | Biotechnology   | Python, R         |
| Nina Julian              | Julian        | anyangonina39@gmail.com    | Listening to Music  | Kenya    | Biotechnology   | R                 |
| Fowowe Toyin             | Toyin         | toyintoyo05@gmail.com      | Reading             | Nigeria  | Biochemistry    | Python            |

---

## **Task 0: Team Formation & Data Representation**
### **Objective**
- Organize team information in a structured data format using **Python or R**.
- Ensure no loops, conditionals, or functions are used.

### **Approach & Implementation**
#### **R Implementation:**
```r
# Load necessary library
data <- data.frame(
  Name = c("Musa Al Hassan Kromah", "Nina Julian", "Fowowe Toyin"),
  Slack_Username = c("Musa", "Julian", "Toyin"),
  Email = c("kromahmusa86@gmail.com", "anyangonina39@gmail.com", "toyintoyo05@gmail.com"),
  Hobby = c("Hiking", "Listening to Music", "Reading"),
  Country = c("Liberia", "Kenya", "Nigeria"),
  Discipline = c("Biotechnology", "Biotechnology", "Biochemistry"),
  Preferred_Language = c("Python, R", "R", "Python")
)
print(data)
```

✅ **Outcome:** A structured data representation successfully printed.

---

## **Task 1: Microbial Growth Curve Analysis**
### **Objective**
- Analyze microbial growth curves for **knockout (-) and knock-in (+) strains**.
- Compute **time to carrying capacity**.
- Visualize data using **scatter and box plots**.
- Perform **statistical analysis**.

### **Approach & Implementation**
#### **Python Implementation:**
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
data = pd.read_csv("microbial_growth.csv")

# Plot growth curves
sns.lineplot(data=data, x="Time", y="OD600", hue="Strain")
plt.title("Microbial Growth Curve")
plt.xlabel("Time (hours)")
plt.ylabel("OD600")
plt.show()
```
✅ **Outcome:** Successfully visualized growth differences between strains.

---

## **Task 2: Advanced Bioinformatics Analyses**

### **2.1 Microbiology: Growth Curve Analysis**
📌 **Objective:** Compare microbial growth rates between knock-out (-) and knock-in (+) strains.
📌 **Implementation:** Used **Python (pandas, matplotlib, seaborn)** for data visualization.

### **2.3 Botany & Plant Science: Metabolic Response Analysis**
📌 **Objective:** Identify key metabolites in pesticide-resistant crops at different time points.
📌 **Implementation:** Used **scatter plots, regression models**, and **residual calculations**.

### **2.4 Biochemistry & Oncology: Protein Mutation Impact**
📌 **Objective:** Analyze mutations affecting both protein structure and function.
📌 **Implementation:** Integrated **SIFT & FoldX datasets**, visualized mutation frequencies using **bar plots and pie charts**.

### **2.6 Transcriptomics: RNA-seq Data Analysis**
📌 **Objective:** Identify **upregulated and downregulated genes**.
📌 **Implementation:** Generated **volcano plots**, analyzed gene expression trends.

### **2.7 Public Health: NHANES Data Analysis**
📌 **Objective:** Evaluate relationships between **BMI, weight, and age**.
📌 **Implementation:** Conducted **t-tests**, plotted **weight-height correlations** using **gender, diabetes, and smoking status** as factors.

---

## **Upcoming Tasks**
📅 More advanced bioinformatics challenges will be added as the internship progresses.

---

## **How to Contribute**
1. **Clone the repository:**
   ```bash
   git clone https://github.com/mkromah/HackBio-BioCoding-Intership.git
   ```
2. **Navigate to the project folder:**
   ```bash
   cd HackBio-BioCoding-Intership
   ```
3. **Work on your assigned task and commit changes:**
   ```bash
   git add .
   git commit -m "Completed Task X"
   git push origin main
   ```

---

## **Contact & Socials**
🔗 **GitHub Repository:** [HackBio BioCoding Internship](https://github.com/mkromah/HackBio-BioCoding-Intership)  
🔗 **LinkedIn Post:** [Follow our progress](https://www.linkedin.com/posts/mkromah_hackbio-bioinformatics-biocoding-activity-7294767807068569600-D8fu)  

🙌 **Happy Coding!** 🚀

