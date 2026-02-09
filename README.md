# Road Project Traffic Survey Data Analysis

## Project Title  
**Construction and Widening of Road from ECB Chattar to Manikdi and Jashimuddin to Uttara 3rd Phase**

---

## Project Overview

This repository contains traffic survey data analysis codes developed for the road project  
**“Construction and Widening of Road from ECB Chattar to Manikdi and Jashimuddin to Uttara 3rd Phase.”**

The analyses are based on field traffic survey data and are intended to support transportation planning, traffic demand assessment, and road capacity evaluation.

All analyses were carried out using **Python** in **Kaggle Notebook**.

---

## Author

**Md. Ausaf Alam**  
Lecturer
Bangladesh Army University of Science and Technology, BAUST

Assistant Engineer, GeoStruct Consultant Limited
M.Sc. in Civil Engineering (Transportation)  
Bangladesh University of Engineering and Technology (BUET)

---

## Data Analysis Components

### 1. Classified Traffic Count (CTC) Analysis  
📄 `ctc-data-analysis.ipynb`  
- Direction-wise traffic volume
- Maximum hourly traffic volum
- K-Factor (Peak Hour Factor)
For each traffic direction, traffic volumes were aggregated for three time periods:
- Morning
- Noon
- Evening

---

### 2. Road Side Interview (RSI) Data Analysis  
📄 `rsi-data-analysis.ipynb`  
- Data Cleaning, mapping with actual names
- Trip purpose distribution
- Age wise travel behavior analysis
- Survey  point wise mode analysis
- Min, Max, Average travel cost/km and Trip length analysis   
- Intra and Interzonal Trip Analysis  

---

### 3. Master Origin–Destination (O–D) Matrix Preparation  
📄 `master-od-matrix-rsi-data.ipynb`  
- Imported required Python libraries and configured file paths  
- Identified and listed RSI location-wise data files, excluding the master file  
- Automatically detected the anchor cell of the O–D matrix in each worksheet  
- Extracted individual **63 × 63 O–D matrices** from each vehicle-type sheet  
- Aggregated O–D matrices from **19 survey locations** across **25 vehicle categories**  
- Compiled and wrote the aggregated matrices into a **master file (sheet-wise by vehicle type)**  
- Saved the final consolidated Master O–D Matrix for further planning and modeling use  
---

### 4. MRT / Traffic Survey Data Analysis  
📄 `mrt-survey-rev-01.ipynb`  
- Survey data cleaning and processing  
- Owned vs non owned vehicle ownership 
-Top Origin Destination from MRT Station 

---

### 5. Pedestrian Count Analysis  
📄 `pedestrian-count-analysis.ipynb`  
- Imported pedestrian survey data and standard template using `openpyxl`  
- Automatically identified valid time-interval rows while ignoring subtotal and text rows  
- Matched time blocks between survey data and template sheets  
- Transferred direction-wise pedestrian counts (P1, P2, PC-1) to designated template columns  
- Assigned zero values where pedestrian categories were not observed  
- Preserved all existing formulas in the template workbook  
- Generated and saved a completed pedestrian count output file for each survey location  

---

## Tools & Technologies Used

- Python  
- Kaggle Notebook  
- Pandas  
- NumPy
- datetime
- OS
- openpyxl
- glob
- Matplotlib / Seaborn   

---

## Application of the Analysis

- Road capacity evaluation  
- Traffic demand assessment  
- Input for traffic simulation models (e.g., VISSIM, TransCAD)  
- Support for feasibility studies and design decisions  

---

## Notes

- Survey data used in this repository are project-specific.  
- The codes are intended for **academic, research, and transportation planning purposes**.  

---

## Contact

GitHub: **@Ausaf99**
Kaggle: **https://www.kaggle.com/ausafalam**
LinkedIn: **https://www.linkedin.com/in/ausaf-alam99/**
