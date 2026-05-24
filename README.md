# data_cleaning_automation2
# Project 4 — Data Cleaning & Reporting Automation
### Thiranex Data Analytics Internship

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Project](https://img.shields.io/badge/Project-04-blue)
![Track](https://img.shields.io/badge/Track-Data%20Analytics-orange)
![Due](https://img.shields.io/badge/Due-29%20May%202026-yellow)

---

## Overview

A fully automated data cleaning and reporting tool built with vanilla JavaScript and Chart.js. Upload any CSV file — the tool automatically detects and fixes data quality issues, generates visual reports, and lets you download a clean dataset and audit report.

---

## Features

- Duplicate Detection — Identifies and removes exact duplicate rows automatically
- Missing Value Handling — Auto-fills empty numeric fields with 0 and empty text fields with "Unknown"
- Format Standardisation — Normalises inconsistent casing (e.g. EAST to East, completed to Completed)
- Date Format Fixing — Converts DD-MM-YYYY and YYYY/MM/DD to standard YYYY-MM-DD
- Invalid Data Detection — Catches non-numeric values in numeric columns and corrects them
- Data Quality Score — Calculates an overall quality score (%) after cleaning
- 4 Visual Charts — Revenue by Region, Orders by Status, Issue Breakdown, Top Products by Revenue
- Download Clean CSV — Export the cleaned dataset as a .csv file
- Download Audit Report — Export a full issue log and audit trail as a .txt file

---

## Tech Stack

Tool              | Purpose
------------------|--------------------------------------------
HTML5 / CSS3      | Structure and styling
Vanilla JavaScript| Data cleaning logic and DOM manipulation
Chart.js 4.4.1    | Data visualisation (bar, doughnut, charts)
Google Fonts      | Typography (Syne, DM Mono, Inter)
FileReader API    | CSV file upload and parsing

No frameworks. No backend. No dependencies to install. Runs entirely in the browser.

---

## How to Run

Option 1 — Open locally
1. Download project4_data_cleaning.html
2. Double-click to open in Chrome, Edge, or Firefox
3. Click "Load Sample Sales Data" or upload your own .csv file

Option 2 — Host on GitHub Pages
1. Upload the .html file to a GitHub repository
2. Go to Settings > Pages > Deploy from branch
3. Share the generated URL as your submission link

Option 3 — Use CodePen
1. Go to codepen.io and create a New Pen
2. Paste the full HTML into the HTML box
3. Click Save and share the pen URL

---

## Project Structure

project4-data-cleaning/
│
├── project4_data_cleaning.html   (Main file — entire app in one file)
└── README.md                     (This file)

---

## Data Cleaning Rules Applied

Issue Type            | Detection Method                        | Fix Applied
----------------------|-----------------------------------------|---------------------------
Duplicate rows        | Exact row match using join key          | Row removed
Missing numeric value | Empty cell in quantity/price/revenue    | Filled with 0
Missing text value    | Empty cell in name/region/status column | Filled with "Unknown"
Inconsistent casing   | Compare vs proper-cased version         | Normalised to Title Case
Invalid numeric       | isNaN() check on numeric columns        | Replaced with 0
Wrong date format     | Regex match on DD-MM-YYYY / YYYY/MM/DD  | Converted to YYYY-MM-DD

---

## Sample Output

After loading the sample sales data (14 rows):

- Raw rows: 14
- Clean rows: 13 (1 duplicate removed)
- Issues fixed: 10+
- Data quality score: 93%
- Charts generated: 4

---

## Expected Outcome (Per Brief)

Requirement                        | Implemented
-----------------------------------|----------------------------------
Handle missing values              | Auto-filled with defaults
Handle duplicates                  | Detected and removed
Handle inconsistent data           | Casing, dates, invalid values fixed
Generate automated reports         | Visual report + downloadable .txt
Visual summaries                   | 4 Chart.js charts with insights

---

## Submission

Project      : 04 — Data Cleaning & Reporting Automation
Track        : Data Analytics
Organisation : Thiranex
Due Date     : 29 May 2026
Status       : Completed Successfully

---

Built with JavaScript + Chart.js | Thiranex Data Analytics Internship 2026
