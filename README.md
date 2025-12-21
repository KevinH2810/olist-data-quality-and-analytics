OLIST E-COMMERCE DELIVERY ANALYSIS
==================================

PROJECT OVERVIEW
----------------

This repository contains an exploratory data analysis of delivery performance using
the Brazilian Olist e-commerce dataset.

The main focus of the project is to understand delivery time patterns, variability,
and potential sources of delay from a customer perspective.

The analysis emphasizes clear reasoning, data validation, and distribution-based
interpretation rather than relying solely on single summary metrics.

DATASET
-------

The project uses the Brazilian E-Commerce Public Dataset by Olist, which includes
information about orders, delivery timestamps, sellers, and customer locations.

Only delivered orders are used for delivery time analysis. Records with missing or
logically inconsistent timestamps are separated and reported instead of being silently
removed.

ANALYSIS OBJECTIVES
-------------------

The analysis is structured into multiple focused objectives:

1. Delivery Time Distribution

   - Understand the typical delivery duration and its variability
   - Define relative fast and slow deliveries using median and interquartile range (IQR)
2. On-Time vs Late Delivery Analysis (planned)

   - Compare actual delivery times with estimated delivery dates
3. Delivery Performance by Location or Seller (planned)

   - Explore whether delivery performance differs across cities or sellers

Each objective is implemented as a separate notebook to keep the analysis clear and
self-contained.

REPOSITORY STRUCTURE
--------------------

data/
  raw/        Original datasets
  reports/    Data quality reports (missing or invalid records)

notebooks/
  00_project_overview.ipynb
  01_delivery_time_analysis.ipynb
  02_on_time_vs_late.ipynb          (planned)
  03_delivery_by_location_or_seller (planned)

NOTES ON METHODOLOGY
--------------------

- Data validation is treated as part of the analysis rather than a preprocessing shortcut.
- Missing or logically inconsistent records are separated for transparency.
- Robust statistics such as the median and interquartile range are used to reduce
  distortion from extreme values.
- Delivery performance is described relative to the observed data distribution rather
  than external benchmarks.

HOW TO NAVIGATE
---------------

If this is your first time viewing the project:

1. Start with notebooks/00_project_overview.ipynb
2. Continue to notebooks/01_delivery_time_analysis.ipynb for the first completed objective
3. Additional notebooks build on this foundation
