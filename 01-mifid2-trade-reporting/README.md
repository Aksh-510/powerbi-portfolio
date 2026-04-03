# MiFID II Trade Reporting Dashboard

## Overview
A Power BI dashboard simulating post-trade regulatory reporting workflows 
under MiFID II. Built using synthetic data inspired by real-world financial 
services experience.

## Business Problem
Under MiFID II, investment firms must report all trades to regulators within 
strict deadlines. Failures in reporting - due to invalid LEIs, missing fields, 
or duplicate submissions - result in regulatory breaches. This dashboard 
monitors reporting quality and flags issues for investigation.

## Dashboard Pages

| Page | Description |
|---|---|
| Overview | KPI summary - total trades, rejection rate, notional value |
| Rejection Analysis | Breakdown of rejections by counterparty and reason |
| Venue & Instrument | Trade volume and notional by venue and instrument |
| Timeline | Monthly trends in trade volume and rejection rate |

## Key Insights
- Overall rejection rate: 18.8% across 500 trades
- DUPLICATE_TRADE_ID and PRICE_OUT_OF_RANGE are the top rejection reasons
- UBS Group AG had the highest rejection count among counterparties
- Rejection rate shows variance across months, peaking in May and October

## Tools & Techniques
- **Power BI Desktop** - report building and publishing
- **DAX** - custom measures (rejection rate, notional aggregations)
- **Power Query** - data type transformations
- **Data modelling** - star schema with DateTable relationship

## Dataset
Synthetic dataset of 500 trades generated for portfolio purposes.
No real or confidential data is used.

📁 [Download dataset](./data/synthetic_trades.csv)

## Screenshots
![Overview](./screenshots/01-overview.png)
![Rejection Analysis](./screenshots/02-rejection-analysis.png)
![Venue & Instrument](./screenshots/03-venue-instrument.png)
![Timeline](./screenshots/04-timeline.png)
