## **Food Loss and Waste Analysis (2000-2024)**

### **Where Reported Loss Concentrates: Pareto Analysis**

**Project Overview:** This project analyses the FAO Food Loss and Waste Database (2000 to 2024) to show where reported food loss concentrates along the supply chain. It uses 21,777 records from 115 countries across 19 supply-chain stages, and the findings are presented in an interactive Tableau Public dashboard. Pareto analysis of high-loss records (reported loss of 20% or more) identifies the stages where they concentrate.

## **Data**

* Data source: Food and Agriculture Organization of the United Nations (FAO). Food Loss and Waste Database. Technical Platform on the Measurement and Reduction of Food Loss and Waste.
* [FAO Food Loss and Waste Database](https://www.fao.org/platform-food-loss-waste/flw-data/en/)
* Date Accessed: 23 October, 2026

**Methodology**

1. The project was to analyse the supply chain stages and commodities with the highest reported food loss.
2. Data collection: Data were obtained from the FAO Food Loss and Waste Database (31,455 records) (accessed 23 October 2026).
3. Data cleaning: Exact duplicates and records with no supply chain stage were removed, leaving 27,884 rows.
4. Analysis: The records for the whole supply chain and the World and regional aggregates were all excluded to avoid errors. The final set consisted of 21,777 records from 115 countries across 19 stages.
5. Loss % was presented as the median by stage, commodity, and year; record counts were shown by country. The median was used because the values are skewed.
6. Visualisation:  Interactive Tableau dashboard.
7. Pareto analysis: the records with a loss of 20% or more were tallied by stage to see where the high-loss records were concentrated.
8. Validation: All the figures have been checked against the raw data, and the limitations of the project were noted.  
Dashboard: https://public.tableau.com/views/FoodLossandWasteAnalysis/FoodLossandWasteAnalysis

**Key Insights**

* The median reported loss is 2.5% across 21,777 records.
* Post-harvest and household stages stand out. Both reach a 15.00% median, followed by Retail at 9.50%. Transport records the lowest loss at 1.00%.
* Among commodities with at least 30 records, Mixed grain (12.00%), Pineapples (11.52%), and Other fruits, n.e.c. (10.85%)  rank highest.
* The number of records by country is uneven. India (1,233 records), Ethiopia (992), and Kenya (909) dominate, which limits country-level comparison.

A Pareto analysis of the 586 high-loss records (20% or more) showed that six of the 19 stages account for 83.6% of them, with Retail the largest at 23%.

[View the interactive Pareto Analysis on Tableau Public]
## **Limitations**

* Medians are not weighted by production volume, so they show reported loss.
* Some countries, commodities, and stages have few records, so their medians are less stable, and years 2022 to 2024 also have fewer records.
* Loss and waste are reported in a single field, `loss_percentage`.
* Whole-supply-chain, World, and regional aggregate rows are excluded to avoid double counting.
* A record is classified as high-loss when its reported loss is 20% or more. This is a project-defined threshold, used only for pareto analysis.

## Repository Contents

```
food-loss-waste-analysis/
├── README.md
├── docs/
│   └── Food_Loss_and_Waste_Analysis_Report.pdf
└── images/
    ├── dashboard.png
    └── pareto.png
```

Made by: Navita Arora

