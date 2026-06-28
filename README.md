# 🏥 Health Care Analysis – Power BI Dashboard

An interactive Power BI dashboard that provides end-to-end visibility into healthcare lab test operations — tracking turnaround times, processing centre performance, department-wise metrics, and patient-level test records.

---

## 📊 Dashboard Pages

### Page 1 – Overview (TAT Summary)
![Overview Page](page1_overview.png)

A high-level summary of all lab tests with key KPIs and geographic breakdowns.

**Key Metrics:**
- **Total Tests:** 324K
- **Total Tests Rejected:** 3K
- **% IN TAT (Turnaround Time):** 84.88%
- **Tests on Hold:** 11
- **Tests Re-Run:** 1.88K
- **Tests OUT TAT:** 49K
- **Tests IN TAT:** 275K

**Visuals:**
- % IN TAT by City (bar chart)
- % IN TAT by Processing Centre (line chart)
- Gender filter: Female | Male | Transgender

---

### Page 2 – Detailed Analysis
![Analysis Page](page2_analysis.png)

Deep-dive analytics across departments, processing centres, age groups, and hourly sample flow.

**Visuals:**
- % IN TAT vs Department Name (line chart)
- % IN TAT by Processing Centre (bar chart)
- % IN TAT by Age Group (bar chart — highlights 0–5 age group in red as lowest performer at ~84%)
- Sample flow chart: Dept → SRA received → Result Entry → Approval (by SRA Hour Slab)

---

### Page 3 – Detailed Page (Patient-Level Data)
![Detailed Page](page3_detailed.png)

A granular drill-down table showing individual test records for audit and investigation.

**Columns include:**
- Test Name, State, Visit No, SIN No, Sex
- Processing Centre, Actual Test Centre
- Age, Approval Status, Booking Centre

---

## 🔍 Filters Available (All Pages)

| Filter | Description |
|--------|-------------|
| Booking Date | Filter by when the test was booked |
| SIN No | Patient SIN number |
| Doctor Name | Referring doctor |
| City | City of sample collection |
| Department Name | Lab department |
| Delivery Date | Expected delivery date |

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Dashboard development |
| **DAX** | KPI calculations (% IN TAT, Re-Run Rate, etc.) |
| **Power Query (M)** | Data transformation & cleaning |
| **Power BI Service** | Publishing & sharing |

---

## 📁 Project Structure

```
healthcare-powerbi/
│
├── HealthCareAnalysis.pbix       # Main Power BI report file
├── README.md                     # Project documentation
├── screenshots/
│   ├── page1_overview.png        # Overview page
│   ├── page2_analysis.png        # Analysis page
│   └── page3_detailed.png        # Detailed data page
└── data/                         # Sample/anonymized data (if applicable)
```

---

## 🚀 How to Use

1. **Download** the `.pbix` file from this repository
2. **Open** it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. Use the **slicers** (Booking Date, Doctor Name, City, etc.) to filter the data
4. Navigate between **Overview → Analysis → Detailed Page** using the navigation buttons
5. Click **"Clear all slicers"** to reset all filters at once

---

## 💡 Key Insights

- Overall TAT compliance stands at **84.88%** across 324K tests
- The **0–5 age group** shows the lowest TAT compliance (~84%), flagging a potential area for operational improvement
- Most cities maintain **~100% TAT compliance**, with a few outliers worth investigating
- **49K tests** missed the TAT window, representing ~15% of all tests — a key metric to optimize

---

## 👤 Author

**Soumen Gupta**  
📧 soumencse20@gmail.com  
🔗 [LinkedIn Profile](https://linkedin.com/in/soumenz2)  
🐙 [GitHub](https://github.com/soumenz2)

---

## 📄 License

This project is for portfolio and educational purposes.
