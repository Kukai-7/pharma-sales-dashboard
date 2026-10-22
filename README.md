# Pharma Sales & P&L Dashboard

A three-page Power BI report on a pharmaceutical distributor's sales and profitability.

## Pages

| Page | What it answers |
|---|---|
| **Executive P&L Overview** | How much did we sell and earn? Net revenue, gross margin, gross profit, units, YoY growth, monthly trend vs prior year, P&L waterfall |
| **Product Performance** | Which products carry the business? Top products by sales, volume and margin, margin vs revenue scatter, filters by brand and category |
| **Regional Performance** | Where is the money made? Revenue and gross profit by region, country-level matrix with margins and YoY |

## Data model

Star schema built in Power Query:

- `FactSales` at the center
- `DimProduct`, `DimPharmacy`, `DimCity`, `DimDate`
- `_Measures`: a dedicated table for all DAX measures (Net Revenue, Gross Margin %, Sales PY, Sales YoY %, top-product measures…)
- `PnL Waterfall`: a helper table driving the waterfall chart

## How to open

Download `Pharma - Visual Data.pbix` and open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows).

## Stack

`Power BI` `Power Query` `DAX`
