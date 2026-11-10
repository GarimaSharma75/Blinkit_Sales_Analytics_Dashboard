# Blinkit Grocery Sales & Outlet Performance Analytics

An interactive **Power BI dashboard** for analysing grocery sales across item categories, outlet sizes, location tiers, and outlet establishment years.



## Dashboard Preview

Save the final screenshot as `Screenshots/Blinkit_Dashboard.png`, then embed it here:

<!-- ![Blinkit Dashboard](Screenshots/Blinkit_Dashboard.png) -->

## Objectives

- Monitor sales performance using KPI cards.
- Compare sales across item categories.
- Analyse sales distribution by outlet size.
- Compare performance across outlet location tiers.
- Explore sales by outlet establishment year.
- Enable interactive filtering with slicers.

## Key Performance Indicators

Current unfiltered values displayed in Power BI (rounded):

| KPI | Displayed value | Definition |
|---|---:|---|
| Total Sales | 1.20M | Sum of Sales |
| Average Sales | 140.99 | Average of Sales |
| Total Items | 9K | Count of item records |
| Average Rating | 3.92 | Average of Rating |

Recheck these values in the final saved report before publishing.

## Dashboard Visuals

| Visual | Purpose |
|---|---|
| Horizontal bar chart | Sales by Item Type |
| Donut chart | Sales distribution by Outlet Size |
| Column chart | Sales by Outlet Location Type |
| Line chart | Sales by Outlet Establishment Year |
| KPI cards | Total Sales, Average Sales, Total Items, Average Rating |
| Slicers | Outlet Location Type, Outlet Size, Item Type |

## Dataset

The CSV contains grocery item and outlet attributes. Expected columns include `Item Fat Content`, `Item Identifier`, `Item Type`, `Item Visibility`, `Item Weight`, `Outlet Establishment Year`, `Outlet Identifier`, `Outlet Location Type`, `Outlet Size`, `Outlet Type`, `Rating`, and `Sales`.

See [Dataset/README.md](Dataset/README.md). The dataset is not included in this starter package; only redistribute it if its licence permits.

## Data Preparation

Data preparation was performed in Power Query Editor. Column types and data quality were reviewed, and a cleaned item fat-content category was created to standardise inconsistent labels. Document the exact final transformation steps after verifying them in Power Query.

## Tools

- Microsoft Power BI Desktop
- Power Query
- DAX
- CSV
- GitHub

## DAX Measures

Example measures (adjust the table name if yours differs):

```dax
Total Sales =
SUM('BlinkIT Grocery Data'[Sales])

Average Sales =
AVERAGE('BlinkIT Grocery Data'[Sales])

Total Items =
COUNTROWS('BlinkIT Grocery Data')

Average Rating =
AVERAGE('BlinkIT Grocery Data'[Rating])
```

## Repository Structure

```text
Blinkit_Sales_Analytics_Dashboard/
├── README.md
├── .gitignore
├── Dataset/
│   └── README.md
├── PowerBI/
│   └── README.md
├── Screenshots/
│   └── README.md
└── Documentation/
    └── Project_Overview.md
```

## How to Use

1. Clone or download this repository.
2. Open `PowerBI/Blinkit_Sales_Analytics.pbix` in Power BI Desktop.
3. If prompted, update the source path to the CSV on your computer.
4. Refresh the report.
5. Use the slicers to explore the data.

## Future Improvements

- Apply a polished purple/lavender theme.
- Refine chart titles, labels, spacing, and slicers.
- Add verified business insights.
- Include final dashboard screenshots.

## Author

**Garima Sharma**  

[GitHub Profile](https://github.com/GarimaSharma75)
[Linkedin Profile]((https://www.linkedin.com/in/garima-sharma-4610a8293/))
---
Academic and portfolio project demonstrating data analysis and dashboard development using Power BI.
