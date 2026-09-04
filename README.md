# 🏥 Hospital Emergency Room Dashboard

An interactive **Power BI** dashboard that monitors emergency room performance — patient referrals, wait times, department load, and satisfaction — built to help hospital operations teams spot bottlenecks and staff more effectively during peak hours.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/status-complete-brightgreen)

---

## 📊 Overview

This project analyzes **9,216 emergency room visits spanning April 2023 – October 2024**, transforming raw patient-level data into a 4-page interactive report. It was built to demonstrate an end-to-end BI workflow: data cleaning in Power Query, KPI calculation with DAX, and dashboard design for a real operational use case.

**Key questions the dashboard answers:**
- How long are patients waiting, and what % are seen within the 30-minute target?
- Which departments receive the most referrals?
- When are the busiest days/hours, to guide staffing decisions?
- How satisfied are patients, and how does that vary over time?
- What do the patient demographics (age, gender, race) look like?

---

## 🖥️ Dashboard Pages

### 1. Consolidated View
Full-period overview: KPI scorecards (patient count, avg wait time, satisfaction score, referrals), admission status split, % seen within 30 minutes, demographic breakdowns, and a day-of-week × hour-of-day demand heatmap.

![Consolidated View](Consolidated%20View%20Dashboard%20Screenshot.png)

### 2. Monthly View
The same KPI layout, filterable by Year and Month, for drilling into a single month's performance.

![Monthly View](Monthly%20View%20Dashboard%20Screenshot.png)

### 3. Patient Details
A searchable, filterable record-level table of individual patient visits.

![Patient Details](Patient%20Details%20Dashboard%20Screenshot.png)

### 4. Key Takeaways
A written summary translating the visuals into plain-language operational insights and recommendations.

![Key Takeaways](Key%20Takeaways%20Screenshot.png)

---

## 📈 Key Insights

- **Average wait time: ~35.3 minutes** — only ~38% of patients were seen within the 30-minute target, flagging a clear area for process improvement
- **Average satisfaction score: ~4.9 / 10**, indicating moderate satisfaction with room to improve patient experience
- **Top referrals:** General Practice (1,840), Orthopedics (995), Physiotherapy (276), Cardiology (248)
- **Busiest days:** Monday, Saturday, Tuesday — with peak hours around 11 AM, 7 PM, 1 PM, and 11 PM, highlighting when extra staffing matters most
- **Admissions are nearly split 50/50** between admitted and not-admitted patients
- **Demographics:** largest age groups are 30–39 and 20–29; largest reported race group is White, followed by African American and multi-racial patients

---

## 🛠️ Tools & Techniques

- **Power BI Desktop** — report design and visualization
- **Power Query** — data cleaning and transformation of the raw CSV (handling nulls, formatting dates, deriving fields)
- **DAX** — custom measures powering the KPI cards, the 30-minute target %, and drill-down visuals
- **Data modeling** — relationships between the fact table and a date dimension table for time intelligence

---

## 📁 Repository Contents

| File | Description |
|---|---|
| `Hospital Emergency Room Dashboard.pbix` | The full Power BI report file |
| `Hospital ER_Data (1).csv` | Source dataset (synthetic ER visit records) |
| `Consolidated View Dashboard Screenshot.png`, `Monthly View Dashboard Screenshot.png`, `Patient Details Dashboard Screenshot.png`, `Key Takeaways Screenshot.png` | Dashboard screenshots |
| `README.md` | This file |

---

## 🚀 Running It Locally

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only)
2. Clone or download this repo, keeping `Hospital Emergency Room Dashboard.pbix` and `Hospital ER_Data (1).csv` in the same folder
3. Open the `.pbix` file — if prompted about the data source, go to **Home → Transform Data → Data Source Settings**, repoint it to your local CSV, then **Refresh**
4. Navigate between the 4 report pages using the tabs at the bottom or the in-report nav buttons



---

