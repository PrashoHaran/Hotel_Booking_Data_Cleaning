# 🧹 Hotel Booking Demand Data Cleaning Project

This project involves cleaning, validating, and enhancing the **Hotel Booking Demand Dataset** sourced from Kaggle. The goal is to produce a high-quality, analysis-ready dataset through a structured data cleaning pipeline, feature engineering, and automated reporting.

---

## 📊 Dataset Overview

- **Source**: [Kaggle - Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- **Rows**: 119,390
- **Columns**: 32
- **Data Range**: July 2015 – August 2017
- **Type**: Mixed (numerical, categorical, datetime)
- **Format**: CSV

---

## ✅ Project Objectives

- Identify and handle missing values, duplicates, and outliers.
- Resolve inconsistencies and logical errors.
- Engineer new features to support analysis.
- Automate the cleaning pipeline for reusability.
- Validate the cleaned data and document all cleaning activities.
- Evaluate data quality improvements with visual dashboards.

---

## 🧽 Cleaning Tasks Performed

### Phase 1: Data Assessment
- Inspected dataset structure, types, and summaries.
- Analyzed missing values, duplicate entries, and inconsistencies.

### Phase 2: Data Cleaning
- Handled missing values with defaults and mode imputation.
- Removed exact duplicate rows.
- Detected outliers using the IQR method.
- Fixed logical errors (e.g., bookings with 0 guests).
- Standardized categorical values and reformatted dates.

### Phase 3: Data Validation and Documentation
- Validated total guest counts, date ranges, and expected value ranges.
- Checked integrity of categorical variables.
- Generated a structured **data cleaning report** summarizing all actions taken.
- Exported the cleaned dataset and created a **data dictionary**.

---

## 🔧 Project Extensions

### Extension 1: Feature Engineering
- Created new features:
  - `total_nights` = weekday + weekend nights
  - `total_guests` = adults + children + babies
  - `revenue` = adr × total nights
  - `season`, `booking_notice_period`, `is_weekend_arrival`

### Extension 2: Automated Cleaning Pipeline
- Developed reusable functions for each cleaning task.
- Combined into a pipeline: `clean_hotel_data()`
- Implemented validation checks via `validate_data()`

### Extension 3: Data Quality Metrics
- Created function `data_quality_summary()` for metric comparison.
- Built before/after visualizations using Matplotlib.
- Evaluated improvements in missing values, duplicates, and invalid rows.

---

