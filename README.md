# 🧹 GameZone Orders – Excel-Based Data Cleaning Project

This project focuses on cleaning and structuring raw e-commerce order data of 20,000 rows from GameZone using **Microsoft Excel**. The raw data was transformed into a clean, analysis-ready format by resolving inconsistencies, standardizing formats, and enriching the dataset with regional data.

---

## 📁 Dataset Contents

**File:** `gamezone-orders-data cleaned data.xlsx`  
**Sheets:**
1. `orders` – Raw e-commerce orders (original)
2. `orders Cleaned` – ✅ Cleaned and structured version
3. `region` – Original country-region reference
4. `region (Cleaned)` – ✅ Validated and enriched country-region mapping
5. `Pivot Table` – ✅ Analytical summaries (e.g., orders by region/platform)
6. `Issue Log` – ✅ Detailed record of identified issues and fixes

---

## ✅ Cleaning Performed (in Excel)

### `orders Cleaned` Sheet:
- Removed duplicate rows based on `ORDER_ID`
- Standardized timestamp formats in `PURCHASE_TS` and `SHIP_TS`
- Normalized values across:
  - `PURCHASE_PLATFORM`
  - `MARKETING_CHANNEL`
  - `ACCOUNT_CREATION_METHOD`
- Verified all `COUNTRY_CODE` entries with the cleaned `region` sheet
- Added calculated fields (e.g., shipping delay, day of purchase)
- Ensured consistent formatting for prices (e.g., decimal places)
- Removed or flagged invalid/null entries where applicable

### `region (Cleaned)` Sheet:
- Verified all country codes against ISO standards
- Added or corrected `REGION` classifications
- May include extra metadata columns (e.g., subregion or validation notes)

---

## 🔄 Pivot Table

Summarizes order data by region, platform, or other categories to support quick analysis.

---

## 🛠 Tools Used

- **Microsoft Excel**
  - Formulas
  - Conditional formatting
  - Data validation
  - Pivot tables

---

## 📌 Sheet Guide

| Sheet              | Description                                      |
|--------------------|--------------------------------------------------|
| `orders`           | Original order data                              |
| `orders Cleaned`   | Final cleaned dataset with 20 fields             |
| `region`           | Raw region mapping                               |
| `region (Cleaned)` | Verified and corrected mapping                   |
| `Pivot Table`      | Summary table for reporting                      |
| `Issue Log`        | List of data issues and how they were resolved   |

---

## ✅ Project Status

- [x] Raw data ingestion
- [x] Cleaning and normalization
- [x] Region mapping and enrichment
- [x] Pivot table summary
- [x] QA and validation

---

**Author:** *Shivam Rana*  
**Last Updated:** May 2025  
**License:** MIT or similar open data license
