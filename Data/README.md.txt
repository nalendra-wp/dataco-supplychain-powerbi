# Dataset Information

This project uses the **DataCo Smart Supply Chain Dataset** (2015–2018), publicly available on platforms such as **Kaggle** (`DataCo SMART SUPPLY CHAIN FOR BIG DATA ANALYSIS` or equivalent DataCo Supply Chain listings).

Inside the Power BI model (`Pbix/`), the data is structured into a star schema (`Fact_Orders`, `Dim_Date`, `Dim_Geography`, `Dim_Customer`, `Dim_Product`) with 12 DAX measures and Row-Level Security roles (`Market_Europe` and `Market_PacificAsia`).

Raw dataset files are omitted from `Data/` due to GitHub file size limits.