# Public School Enrollment Tool

> **Note:** This repository serves as the official **Issue Tracker and Feedback Hub** for the Public School Enrollment Tool. The application source code is managed separately.

[![Launch App](https://img.shields.io/badge/Launch-Dashboard-blue?style=for-the-badge&logo=rstudio)](YOUR_APP_URL_HERE)
[![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)]()

## 📊 About the Tool

The **Public School Enrollment Tool** is an interactive R Shiny dashboard designed for researchers, policymakers, and the public to visualize shifts in U.S. public school enrollment from 2000 to 2023.

By integrating data from the **National Center for Education Statistics (NCES)** and the **Urban Institute's Education Data Portal**, the tool allows users to analyze trends at three geographic levels:

1.  **National (State Level):** Compare total enrollment changes across all 50 states (sourced from NCES Digest).
2.  **Regional (County Level):** View aggregate enrollment for all schools within county boundaries.
3.  **Local (District Level):** Drill down into Unified School Districts (LEAs).

### Key Features
* **Longitudinal Analysis:** Compare enrollment data between any two years from 2000–2023.
* **Interactive Mapping:** Click-to-zoom functionality for drilling down from State to County views.
* **Smart Metrics:** Automatic calculation of net change and percent change.
* **Data Transparency:** Clear distinction between datasets that include Pre-Kindergarten (State) and those that do not (Local).

---

## 🐛 How to Report Issues

We use this repository to track bugs, feature requests, and general feedback. If you encounter an error or have an idea for improvement, please use the **[Issues Tab](../../issues)**.

### Before Submitting
1.  **Check Existing Issues:** Look to see if someone else has already reported your problem.
2.  **Check the App Roadmap:** Navigate to the "Roadmap" tab inside the dashboard to see if your feature is already planned (e.g., Charter School filters or Data Export).

### Submitting a Bug Report
When opening a new issue, please include:
* **Description:** What were you trying to do?
* **Steps to Reproduce:** e.g., "1. Select 'County View'. 2. Click on Texas. 3. Move slider to 2005."
* **Expected vs. Actual:** What should have happened vs. what actually happened.
* **Screenshots:** If possible, include a screenshot of the error or map glitch.

### Submitting a Feature Request
* Describe the feature you would like to see.
* Explain *why* this feature would be useful for your research or analysis.

---

## 🗺️ Roadmap & Known Limitations

Please review the **Roadmap** tab within the live application for the most up-to-date status on upcoming features.

**Current Priorities:**
* ✅ **v1.1 (Live):** High-resolution mapping and data sourcing updates.
* 🚧 **Q1 2025:** Data Export functionality (.CSV/.GeoJSON).
* 🚧 **Q1 2025:** Charter School inclusion/exclusion toggles.

**Known Limitations:**
* **County Loading Times:** Generating county aggregates requires fetching individual school records via API, which may take 5–10 seconds per state.
* **Territories:** Puerto Rico, Guam, and other territories are currently excluded due to map data availability.

---

## 📄 Data Sources

* **State Estimates:** [NCES Digest of Education Statistics, Table 203.20](https://nces.ed.gov/programs/digest/d24/tables/dt24_203.20.asp)
* **Local Data:** [Urban Institute Education Data Portal (CCD)](https://educationdata.urban.org/documentation/)
* **Geography:** U.S. Census Bureau TIGER/Line Shapefiles via the `tigris` R package.

---

*Maintained by the Josh DeLaRosa.*
