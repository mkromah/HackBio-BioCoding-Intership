# **HackBio Internship – BioCoding**

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

👉 **Outcome:** A structured data representation successfully printed.

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
```

---

## **Task 2: Advanced Bioinformatics Analyses**
### **Objective**
- Perform computational analyses in various biological disciplines.
- Apply data science, visualization, and statistical modeling techniques.

### **2.1 Microbiology: Growth Curve Analysis**
🔹 **Objective:** Analyze microbial growth under different conditions.

🔹 **Approach:** Used Python to process growth curve data, visualize trends, and determine significant differences.

#### **Python Implementation:**
```python
# Import necessary libraries
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load growth curve data
data = pd.read_csv("growth_curve_data.csv")

# Plot microbial growth
g = sns.lineplot(data=data, x="Time", y="OD600", hue="Condition")
g.set(title="Microbial Growth Curve", xlabel="Time (hours)", ylabel="Optical Density (OD600)")
plt.show()
```

---

### **2.3 Botany & Plant Science: Metabolic Response Analysis**
🔹 **Objective:** Evaluate metabolic shifts in response to environmental changes.

🔹 **Approach:** Used R for data normalization and visualization.

#### **R Implementation:**
```r
# Load required library
library(ggplot2)

# Read dataset
data <- read.csv("metabolic_data.csv")

# Generate boxplot
p <- ggplot(data, aes(x=Condition, y=Metabolite_Level, fill=Condition)) +
     geom_boxplot() +
     ggtitle("Metabolic Response Analysis")
print(p)
```

---

### **2.4 Biochemistry & Oncology: Protein Mutation Impact**
🔹 **Objective:** Assess functional impact of protein mutations.

🔹 **Approach:** Python-based structural modeling and variant impact prediction.

#### **Python Implementation:**
```python
from Bio.PDB import *

# Load PDB file
parser = PDBParser()
structure = parser.get_structure("Protein", "protein_structure.pdb")

# Extract chain A
chain_A = structure[0]["A"]

# Print residue names
for residue in chain_A:
    print(residue.resname)
```

---

### **2.6 Transcriptomics: RNA-seq Data Analysis**
🔹 **Objective:** Perform differential expression analysis on RNA-seq data.

🔹 **Approach:** Used Python and R to preprocess and analyze RNA-seq datasets.

#### **Python Implementation:**
```python
import pandas as pd
import seaborn as sns

# Load RNA-seq data
data = pd.read_csv("rna_seq_data.csv")

# Generate heatmap
sns.heatmap(data.corr(), cmap="coolwarm", annot=True)
plt.title("Gene Expression Correlation")
plt.show()
```

---

### **2.7 Public Health: NHANES Data Analysis**
🔹 **Objective:** Investigate health trends using NHANES dataset.

🔹 **Approach:** Statistical analysis in Python to uncover population health insights.

#### **Python Implementation:**
```python
import pandas as pd

# Load NHANES dataset
data = pd.read_csv("nhanes_data.csv")

# Summary statistics
print(data.describe())
```

