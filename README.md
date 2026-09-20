# Hotel Bar Inventory Demand Forecasting

## Overview

This project develops a demand forecasting and inventory replenishment
solution for a hotel chain with multiple bars and alcohol brands.

## Business Problem

The hotel experiences both stockouts and overstocking.

The objective is to analyze historical consumption, forecast demand,
calculate appropriate inventory Par Levels, and simulate replenishment.

## Approach

1. Data loading and validation
2. Exploratory data analysis
3. Daily Bar-Brand demand aggregation
4. Demand forecasting
5. Par Level calculation
6. Inventory simulation

## Forecasting

Two approaches were evaluated:

- 7-day moving-average baseline
- Exponential Smoothing

Evaluation metrics:

- MAE
- WAPE

## Inventory Logic

Par Level = Lead-Time Demand + Safety Stock

Assumptions:

- Lead time: 2 days
- Z-value: 1.645
- Approximately 95% one-sided service level

## Results

- Total recommended Par Level: 42,505.65 ml
- Simulation records: 7,104
- Stockout events: 396
- Lost volume: 49,404.91 ml

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Statsmodels
- Matplotlib
- Seaborn

## Future Improvements

- Use actual supplier lead times
- Model delivery delays explicitly
- Improve item-level forecasting
- Add dynamic reorder points
- Add production monitoring
