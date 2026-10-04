# Transportation Network Volume Forecasting & Optimisation
> Analysed daily transportation volumes and capacity across a European e-commerce network, built a forecasting model, and developed data-driven recommendations to improve network planning and reduce operational risk.

## **View the Full Project →**

## About the Project

ABC Buy is a fictional large-scale European e-commerce company operating a multi-node fulfilment and transportation network across Germany, France, Poland, Italy, Spain, the Netherlands, Belgium, Luxembourg and other key markets.

This project investigates daily package volumes, capacity utilisation and forecast accuracy across 58 nodes, 16 carriers and 220 lanes over an 18-month period (January 2024 – June 2025). The goal was to give transportation planners clear visibility into historical performance, identify hidden capacity risks, and generate a reliable forward-looking volume forecast.

## Objective

The objective was to:

- Build a reliable daily volume forecasting capability for the European transportation network.
- Measure capacity utilisation and identify lanes with high overload risk.
- Quantify forecast accuracy (MAPE) across peak, non-peak and seasonal periods.
- Highlight volume concentration by country and node type.
- Translate the findings into practical recommendations for proactive capacity planning.

## Project Approach

The investigation followed a structured end-to-end analytics approach:

**Business Question → Data Ingestion & Modelling (S3 + Glue + Athena) → Exploratory Analysis & KPI Development → Volume Forecasting (SageMaker + Prophet) → Bottleneck & Utilisation Analysis → Dashboard & Visual Insights → Strategic Recommendations**

This allowed the analysis to move from raw operational data to a complete decision-support solution covering historical performance, predictive forecasting and actionable recommendations.

## Technical Stack

**Data Generation & Preparation**
- Synthetic realistic logistics data generation
- Python
- Data modelling (star-schema style)

**Cloud Data Architecture (AWS)**
- Amazon S3 (raw + processed zones)
- AWS Glue Data Catalog
- Amazon Athena
- Partitioned data design and external tables
- Cleaned analytical views

**Forecasting**
- Amazon SageMaker (Notebook Instance)
- Prophet time-series model
- Volume forecast with confidence intervals
- Forecast results written back to S3 (CSV + Parquet)

**Business Intelligence**
- Power BI Desktop
- Star-schema data model
- DAX measures (volume, utilisation, MAPE, forecast metrics)
- Interactive 3-page dashboard (Executive Overview, Network Performance, Forecast)

## Key Result

The analysis showed that the network handled approximately **115 million packages** over the period, with average capacity utilisation of **64.3%** and overall forecast accuracy (MAPE) of **8.07%**.

While average metrics appeared healthy, several important risks were uncovered:
- Certain lanes regularly experienced utilisation spikes above **170–180%**.
- Forecast error increased significantly during summer months (MAPE above 10%), while peak periods delivered better accuracy (MAPE 6.32%).
- Volume was heavily concentrated in Germany and in Fulfilment Centres (nearly half of all volume).

A Prophet forecast was produced to support proactive capacity planning. The findings led to three focused recommendations: prioritise high-spike lanes, improve seasonal forecast calibration, and concentrate capacity attention on the highest-volume nodes and countries.

## Data

This project uses a **real-world style synthetic dataset** created specifically for portfolio purposes. It does not contain real company, customer, or confidential commercial data.

## Full Project

The complete case study contains the detailed business context, analytical approach, key insights, strategic recommendations, expected business impact, technical implementation, dashboard, and lessons learned.

## **View the Full Project →**
