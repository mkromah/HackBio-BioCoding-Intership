# HackBio Internship - Team BioCoders (R Implementation)   

This repository contains solutions for the **HackBio Internship** Task 1, completed by **Team BioCoders** using **R**. The project covers fundamental bioinformatics and computational biology tasks, including **DNA-to-protein translation, bacterial growth modeling, carrying capacity estimation, and Hamming distance calculation**.  

## Task Overview

### 1. DNA to Protein Translation 
Using the **Biostrings** package, we implemented a function to translate a given **DNA sequence** into a **protein sequence** using the standard genetic code.  
- **Method:**  
  - The function takes a DNA sequence as input.  
  - It uses `DNAString()` from Biostrings to process the sequence.  
  - The `translate()` function converts it into a protein sequence.  
- **Example Output:**  
  - Input: `"ATGCCTGAGGAGTAA"`  
  - Output: `"MPERV*"`  

### **2. Logistic Growth Curve Simulation**  
We modeled **bacterial growth** using the **logistic growth equation**, plotting different growth curves with **randomized growth rates** and **lag phase durations**.  
- **Key Features:**  
  - Simulated bacterial population growth with a **carrying capacity of 200**.  
  - Created **100 different growth curves** by randomizing growth rates and lag phase midpoints.  
  - Used R’s `plot()` function to visualize bacterial growth over time.  

### **3. Carrying Capacity Estimation**  
A function was developed to determine the **carrying capacity** of a bacterial population by calculating the **time required** to reach a given percentage of maximum population size.  
- **Method:**  
  - Uses the logistic growth equation to **estimate the time required** for a population to reach 80% of its carrying capacity.  
- **Validation:**  
  - Tested at **growth rate = 0.5**, **midpoint = 40** to confirm correctness.  

### **4. Hamming Distance Calculation**  
We implemented a function to compute the **Hamming distance** between two strings, which measures the number of differing characters.  
- **Key Features:**  
  - Compares two strings **character by character**.  
  - Outputs the **number of positions** where the strings differ.  
  - Handles cases where strings have different lengths.  

## **How to Run the Code**  
1. Install necessary dependencies:  
   ```r
   install.packages("BiocManager")
   BiocManager::install("Biostrings")
   ```
2. Load the script in R and run the functions to test DNA translation, bacterial growth modeling, carrying capacity estimation, and Hamming distance calculation.  

## **Repository Link**  
🔗 **[HackBio Internship - Team BioCoders (R)](https://github.com/mkromah/HackBio-BioCoding-Intership/blob/main/Task%201)**  
