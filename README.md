# DataCo Supply Chain Power BI Dashboard

End-to-end Power BI analytics solution built on the **DataCo Supply Chain** dataset (2015–2018), structured around a star schema (`Fact_Orders`, `Dim_Date`, `Dim_Geography`, `Dim_Customer`, `Dim_Product`) with **12 DAX measures**, a **Clean Teal** visual theme (`Segoe UI`), and **Row-Level Security (RLS)** (`Market_Europe` and `Market_PacificAsia`).

## Dashboard Pages & Previews

### 1. Annual Performance & KPI Summary (2015–2018)
Summarizes key commercial, logistics SLA, and risk metrics across 2015–2018 alongside total figures and scope/methodology notes.

![Annual Performance & KPI Summary](Images/kpi-summary-table.png)

### 2. Executive Commercial & Profit Overview
Tracks overall commercial scale and profitability across segments, time periods, and product categories (`$32M` Net Revenue, `$4M` Total Profit, `12%` Profit Margin, `18.7%` Loss-Making Orders).

![Executive Commercial & Profit Overview](Images/executive-overview.png)

### 3. Supply Chain & Logistics SLA
Monitors shipping performance across markets and shipping modes (`57.3%` Late Delivery Rate, `0.57` Avg Shipping Delay Days, `66K` Orders Shipped).

![Supply Chain & Logistics SLA](Images/logistics-sla.png)

### 4. Order Risk & Fraud
Highlights financial exposure and fraud patterns across markets, order statuses (`SUSPECTED_FRAUD` and `CANCELED`), and payment methods (`$1M` Revenue at Risk, `2.26%` Fraud Rate).

![Order Risk & Fraud](Images/order-risk-fraud.png)

## Row-Level Security (RLS)
Role-based access is configured for regional markets (`Market_Europe` and `Market_PacificAsia`). Below is a preview filtered under the `Market_Europe` role (`$421K` Revenue at Risk, `2.30%` Fraud Rate):

![Row-Level Security - Market_Europe](Images/rls-market-europe.png)

## Repository Structure

├── Data/          # Dataset source notes (README.md)
├── Images/        # Dashboard and RLS preview screenshots (.png)
├── Pbix/          # Power BI report file (.pbix)
└── README.md      # Project documentation

## Key Technical Highlights
- **Data Modeling:** Star schema separating transactional order facts from date, geography, customer, and product dimensions.
- **DAX Measures:** 12 standardized measures grouped across commercial performance, logistics SLA, and order risk/fraud monitoring.
- **Security & Governance:** Role-based filtering via `Market_Europe` and `Market_PacificAsia`.
```[cite: 2, 10, 11, 12]

---

### Urutan Singkat di Lokal Sebelum Upload
1. Pastikan di dalam folder `Data/` hanya ada **`README.md`** (bukan `README.md.txt` dan bukan file CSV raksasa).
2. Pastikan di folder utama ada **`README.md`**, folder **`Data/`**, folder **`Images/`** (isi `.png`), dan folder **`Pbix/`** (isi `.pbix`).
3. Upload semuanya ke repositori GitHub `nalendra-wp` (`dataco-supplychain-powerbi`).

Sudah beres dibuat dua file `.md` tersebut di lokal?