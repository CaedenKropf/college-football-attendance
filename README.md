# College Football Attendance and Enrollment Analysis

This project analyzes factors that influence average home attendance at Division I college football games. Using publicly available football statistics and federal higher-education data, the analysis examines whether team success, enrollment size, gender composition, and conference affiliation help explain variation in attendance across programs.

The project was completed for **BAIS 3250** and is fully reproducible using the files in this repository.

---

## Repository Structure

### 📁 Code
- **Project Scraping (Run First).ipynb**  
  Collects and cleans raw data. This notebook:
  - Scrapes average home attendance and team records from **CFBStats**
  - Pulls institutional enrollment data from **IPEDS** via the Urban Institute API
  - Standardizes names, locations, and identifiers
  - Produces intermediate and cleaned datasets

- **Insights (Run Second).ipynb**  
  Performs all analysis and visualization, including:
  - Correlation and regression analysis
  - Scatterplots with team logos
  - Conference-level attendance comparisons
  - Generation of figures used in the final report

---

### 📁 Data
- **cfbstats_conference_attendance.csv**  
  Raw attendance and team record data scraped from CFBStats.

- **ipeds_directory_plus_enroll.csv**  
  Institutional demographic data from IPEDS, including total undergraduate enrollment and gender breakdowns.

- **cfb_attendance_with_locations.csv**  
  Intermediate dataset combining attendance with stadium and location metadata.

- **final_college_cleaned.csv**  
  **Final cleaned dataset** used for all statistical analysis and visualizations in the project.

- **cfbd.csv**  
  Team identifiers, colors, and branding metadata used for visualization.

- **locations.csv**  
  Stadium and geographic metadata used to align institutions and teams.

---

### 📁 Assets
- **logos/**  
  Folder containing official team logo image files.  
  Logos are sourced from the CFBD GitHub repository:  
  https://github.com/CFBD/cfb-web  

  Logos are matched to teams using numeric identifiers and are used as plot markers in visualizations.

---

### 📄 Report
- **BAIS 3250 Final Project Report.docx**  
  Written report containing the introduction, data description, analysis, results, and conclusions.  
  All figures and statistics referenced in the report are generated directly from the included code.

---

## How to Run the Project

1. Clone or download the repository.
2. Ensure all files remain in the same directory structure.
3. Run **Project Scraping (Run First).ipynb** to reproduce the cleaned dataset.
4. Run **Insights (Run Second).ipynb** to generate all analysis and figures.

> Note: The analysis can also be reproduced directly from `final_college_cleaned.csv` without rerunning the scraping step.

---

## Data Sources

- **CFBStats** – Game-level attendance and team records  
  https://cfbstats.com  

- **IPEDS (Urban Institute API)** – Enrollment and institutional demographics  
  https://educationdata.urban.org  

- **CFBD GitHub Repository** – Team identifiers, logos, and branding  
  https://github.com/CFBD/cfb-web  

---

## Methods Summary

- Average home attendance calculated from home games only
- Win percentage derived from official season records
- Enrollment ratios computed using undergraduate enrollment counts
- Relationships evaluated using correlation analysis and linear regression
- Visualizations include regression lines and logo-based scatterplots

---

## Notes

- Only variables included in the final dataset are documented and analyzed.
- Service academies and select transitioning programs were excluded where appropriate.
- Logos are used solely for visualization clarity.

---

## Author

**Caeden Kropf**  
University of Iowa – Tippie College of Business  
BAIS 3250
