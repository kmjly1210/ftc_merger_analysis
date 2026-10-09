# FTC Merger Enforcement and HSR Transactions

## Research Question
How has FTC merger enforcement activity changed over time relative to
HSR transaction volume, and how has enforcement varied across industries?

## Data
Source: Federal Trade Commission
https://www.ftc.gov/policy-notices/open-government/data-sets

Raw files:
- HSR-Transactions-Filings-Second-Requests-by-FY.csv
- ftc_enforcement.csv

The analysis uses TransactionsReported from the annual HSR dataset
and public FTC merger enforcement records for FY1996–2020.

Annual HSR data replaced the initially planned monthly data to use
a consistent measure of transaction volume.

## Files
- analyis.ipynb: All data cleaning and analysis code.
- data/raw/: Original datasets and source dictionaries.
- data/cleaned/: Cleaned datasets and summary tables.
- data_dictionary.csv: Definitions of derived variables.
- figures/: Analysis charts.
- Final project.pdf: Research report.

## How to Run
1. Download the repository files.
2. Open analyis.ipynb in Google Colab.
3. Run the cells in order from top to bottom.
4. At the file upload prompt, select BOTH original CSV files:
   HSR-Transactions-Filings-Second-Requests-by-FY.csv
   and ftc_enforcement.csv.
5. Continue running the remaining cells to reproduce the analysis,
   charts, and exported CSV files.

Required Python libraries: pandas, matplotlib, and seaborn.

## Analysis
Annual trends, year-over-year percentage changes, enforcement actions
per 1,000 HSR transactions, industry shares, enforcement type shares,
and Pearson correlation.

Period comparisons cover FY1996–2007 and FY2008–2020.

## Limitations
Actions per 1,000 transactions is a descriptive ratio, not an individual
transaction's probability of enforcement. Transaction reporting and
enforcement may occur in different years.

Industry comparisons show enforcement shares because industry-level
HSR transaction counts are unavailable. Correlation does not establish
causation.
