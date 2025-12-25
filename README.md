# USA-Healthcare-Analytics-Dashboard-PowerBI-
This project analyses Healthcare visit data for multiple hospitals and clinics across USA to gain insights on patient behaviour, clinical performance, payment methods and cost distribution.
The dashboard is designed to support: 
  a. Hospital administrators
  b. Clinical Operation Managers
  c. Healthcare Finance teams
by answering key questions around, who is being treated, where, how often and at what cost.

**Business Questions Addressed**
The analysis focuses on answering the following:
  - How many unique patients are being treated over time?
  - Which departments and clinics handle the highest visit volumes?
  - What is the split between new vs returning patients?
  - How do treatment costs vary by department and doctor?
  - What payment methods are most commonly used, and how do they trend?
  - Are certain departments serving specific age groups more heavily?
  - Which visits represent high-cost outliers that may require review?

Key KPIs Tracked
  - Total Unique Patients
  - Total Visits
  - Total Treatment Cost
  - Average Treatment Cost per Visit
  - Returning Patient Percentage
  - Average Patient Age

**Data Model**

The dataset is modeled using a star schema for optimal performance and clarity.
**Fact Table**
Fact_Visit
- Visit_ID
- Visit_Date
- Treatment_Cost
- Payment_Method
- Insurance_Coverage
- Foreign keys to dimensions

**Dimension Tables**
- Dim_Patient (Patient_ID, Age, Gender)
- Dim_Doctor (Doctor_ID, Specialization, Department)
- Dim_Hospital (Hospital_Name, City, Hospital ID)
- Dim_Date
Relationships are one-to-many from dimensions to the fact table, following Power BI best practices.

**Dashboard Pages & Insights.**
**Overview Page**
Purpose: Executive snapshot of healthcare activity

Highlights:
-  Overall patient volume and treatment cost
-  Gender-based patient distribution
-  Payment method share (Insurance vs Out-of-Pocket)
-  Clinic/department visit distribution
-  Time trends in visits and payment methods

**Clinical Performance Page**
Purpose: Operational and clinical efficiency analysis

Key visuals:
- New vs Returning Patients by Department
- Total Visits and Total Treatment Cost by Department
- Doctor Workload vs Average Treatment Cost (scatter plot)
- Department visit trends over time
- Patient age distribution by department
- Top high-cost visits for review

This page helps identify:
- High-pressure departments
- Cost-intensive specialties
- Chronic care vs first-time treatment patterns

**Visit Trends Page**
Purpose: Time-based and facility-level analysis

Key insights:
- Visit volume by hospital
- Patient trends over time (yearly, monthly)
- Decomposition of total visits into new vs returning patients and departments
- Identification of facilities driving the most activity

**Tools & Technologies applied**
- Power BI
- DAX (Measures for KPIs, percentages, trends)
- Data Modeling (Star Schema)
- Healthcare Analytics Concepts

**Dashboard Previews**
<img width="557" height="289" alt="image" src="https://github.com/user-attachments/assets/ead80805-b46f-40bd-bfac-1efe16dec75e" />
<img width="921" height="658" alt="Screenshot 2025-12-25 010827" src="https://github.com/user-attachments/assets/a22ee489-58ba-457a-bcec-1809c82cb722" />
<img width="948" height="577" alt="Screenshot 2025-12-25 011148" src="https://github.com/user-attachments/assets/50f7e5ae-e6fe-41ef-bdc0-3ed6186136dd" />
<img width="1152" height="607" alt="Screenshot 2025-12-25 035735" src="https://github.com/user-attachments/assets/0d5543a8-3273-4d97-b5a8-3f69207c7fce" />

**Key Takeaways**
- Oncology and Pediatrics generate the highest treatment costs.
- There has been a continuous decline in overal patients footfall since Mid 2024 into 2025 indicating reduced demand or access issues. A further deep dive with CX department is needed.
- Certain departments (e.g., Neurology, Oncology) show higher returning patient ratios, indicating chronic care demand.
- Insurance remains the dominant payment method, but out-of-pocket payments show seasonal fluctuations.
- Doctor workload does not always correlate with higher average treatment cost, highlighting efficiency differences.

**Author:**
Robert Kioko M
