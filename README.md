# Excel-Customer-Demographics-amp-Sales-Dashboard

## 📌 Project Overview

This project presents an interactive **Excel Dashboard** built from raw customer demographic data to analyze purchasing behavior and demographic trends. The project demonstrates a full end-to-end data analyst workflow—including raw data cleaning, feature engineering, data aggregation with pivot tables, and dynamic dashboard creation using interconnected slicers.

---

## File

[Excel Project Dataset.xlsx](https://github.com/user-attachments/files/34059896/Excel.Project.Dataset.xlsx)


## 📊 Dataset Overview

The project uses a customer demographic dataset containing key socio-economic and behavioral attributes:

* **Demographics:** Age, Gender, Marital Status, Education, Occupation, Region, Children, Income.
* **Behavioral &amp; Geographic Data:** Commute Distance, Home Owner status, Purchased Bike (Yes/No).

---

## 🛠️ Key Project Phases

### 1\. Data Cleaning &amp; Preprocessing

* **Raw Data Preservation:** Backed up original data to a dedicated working sheet (`Working_Data`) prior to editing.
* **Deduplication:** Identified and eliminated duplicate customer records using Excel's built-in duplicate removal tools.
* **Value Standardization:** Applied `Find &amp; Replace` to standardize single-letter codes into full descriptors (e.g., `M` ➔ `Married`, `S` ➔ `Single`, `M` ➔ `Male`, `F` ➔ `Female`).
* **Numeric Formatting:** Standardized monetary fields to currency formatting and removed unnecessary decimal places.
* **Text Label Optimization:** Replaced misaligned text ranges (e.g., updating `10 miles plus` to `More than 10 miles`) so pivot chart categories sort logically rather than alphabetically.

### 2\. Feature Engineering

* **Demographic Binning:** Engineered a custom `Age Status` column using nested `IF` formulas to group continuous age data (ranging from 25 to 89) into actionable categories:
  * **Adult** (&lt; 35)
  * **Middle Age** (55)
  * **Old** (55+)

### 3\. Data Aggregation &amp; Analysis (Pivot Tables)

Created focused **Pivot Tables** to extract core business metrics:

* **Income Analysis:** Evaluated average income levels broken down by gender and purchase decision.
* **Commute Distance Trends:** Analyzed bike purchasing rates relative to customer commute distances.
* **Demographic Distribution:** Tracked purchase counts across age brackets.

### 4\. Interactive Dashboard &amp; Visualization

* **Layout &amp; Design:** Built a dedicated, gridline-free `Dashboard` tab featuring clean header blocks and styled chart elements.
* **Pivot Charts:** Added formatted clustered column and line charts with custom titles and clear axis labels.
* **Interactive Slicers:** Integrated interactive **Slicers** (`Marital Status`, `Region`, `Education`).
* **Cross-Filtering:** Connected slicers to all underlying pivot tables using **Report Connections**, enabling unified, multi-chart dynamic filtering.

---

## 📁 Repository Structure

```
├── Excel_Customer_Dashboard.xlsx   # Main Excel file containing raw data, pivot tables &amp; dashboard
├── README.md                       # Project documentation
└── assets/                         # Dashboard screenshots &amp; previews
```
