# Website Traffic Analysis

## Project Overview

This project analyzes website traffic event data using Python. The analysis focuses on event activity, daily traffic trends, geographic distribution, content/link performance, artist and track performance, and an event-level engagement measure.

The project is based on the supplied `Website_Traffic_Analysis_Internship.ipynb` notebook.

## Dataset Summary

- **Rows:** 226,278
- **Columns:** 9
- **Date range:** 19 August 2021 to 25 August 2021
- **Unique countries:** 212
- **Unique cities:** 11,993
- **Unique artists:** 2,420
- **Unique tracks:** 3,563
- **Unique links:** 3,839

### Columns

`event`, `date`, `country`, `city`, `artist`, `album`, `track`, `isrc`, `linkid`

## Tools Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib

## Analysis Workflow

1. Import Python libraries.
2. Load `traffic.csv`.
3. Inspect shape, columns, sample rows and data types.
4. Check missing values and exact duplicates.
5. Convert and clean fields.
6. Summarize the dataset.
7. Analyze event distribution.
8. Analyze daily traffic.
9. Analyze countries and cities.
10. Analyze content links.
11. Analyze artists and tracks.
12. Calculate event-level engagement.
13. Document session/user-level limitations.
14. Produce insights and business recommendations.

## Key Results

### Event Distribution

| Event | Count | Percentage |
|---|---:|---:|
| Pageview | 142,015 | 62.76% |
| Click | 55,732 | 24.63% |
| Preview | 28,531 | 12.61% |

The notebook defines event-level engagement as:

`(clicks + previews) / total events`

Result: **37.24%**

### Daily Traffic

- Peak: **19 August 2021 — 35,361 events**
- Lowest: **23 August 2021 — 29,808 events**

### Top Countries

1. Saudi Arabia — 47,334 events
2. India — 42,992
3. United States — 32,558
4. France — 15,661
5. Iraq — 8,260

### Top Content

The highest-volume content link is associated with **Tesher — Jalebi Baby**, with **40,841 total events**.

### Data Quality

The notebook reports:

- **103,711 exact duplicate rows**
- **45.83% duplicate percentage**
- **7,121 missing ISRC values (3.15%)** before cleaning

Exact duplicates are retained because the available fields do not prove whether repeated records are valid repeated events or duplicate ingestion.

## Important Limitation

The supplied dataset does **not** contain:

- User IDs
- Session IDs
- Event timestamps
- Page URLs
- Referral sources
- Explicit conversion events

Therefore, the project does not claim to calculate reliable:

- Unique users
- Sessions
- Bounce rate
- Average session duration
- User journeys
- Entry pages
- Exit pages
- Referral-source performance
- Conversion rate

## Charts to Include in the Report

The final report contains clearly marked placeholders. Recommended charts/screenshots:

1. **Website Event Distribution** — put in the Event Analysis section.
2. **Daily Website Traffic** — put in Daily Traffic Analysis.
3. **Top 10 Countries by Website Activity** — put in Geographic Analysis.
4. **Top 10 Cities** — optional.
5. **Top 10 Content Links by Total Events** — put in Content and Link Performance.
6. **Top 10 Artists by Event Volume** — put in Artist and Track Performance.
7. **High-Engagement Content** — optional, after Engagement Analysis.
8. **Dataset Preview Screenshot** — put in Dataset Description.
9. **Missing Values / Duplicate Check Screenshot** — put in Data Quality Assessment.

## How to Run

Keep the notebook and dataset in the same folder:

```text
project-folder/
├── Website_Traffic_Analysis_Internship.ipynb
└── traffic.csv
```

Open the notebook in Jupyter Notebook or JupyterLab and run the cells from top to bottom.

## Project Structure

```text
Website_Traffic_Analysis/
├── Website_Traffic_Analysis_Internship.ipynb
├── traffic.csv
├── Website_Traffic_Analysis_Internship_Report.docx
├── Website_Traffic_Analysis_Internship_Report.pdf
└── README.md
```

## Recommendations

The notebook recommends:

- Prioritizing high-performing content.
- Focusing on high-activity markets such as Saudi Arabia, India and the United States.
- Improving content recommendations.
- Adding better user/session tracking.
- Conducting A/B testing for layouts, calls-to-action and content placement.

## Source Note

This README and the accompanying report are based on the supplied notebook and its recorded outputs. Future-scope suggestions are recommendations, not measured results.
