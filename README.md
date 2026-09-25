# Restaurant Menu Optimisation with Power BI

## Overview

This project uses sales data from a family-run Chinese restaurant in Fuengirola, Spain, to support practical menu decisions. The goal was to steer demand towards dishes that customers like and the kitchen can prepare more easily, reducing pressure on staff. I cleaned and prepared the data in Excel and built the analysis and dashboard in Power BI.

The sales data shared publicly have been anonymised while preserving relative proportions.

## Business problem

A large menu and uneven demand made kitchen work difficult to manage. Some dishes required considerable effort despite limited demand. The restaurant wanted to promote popular, easier-to-prepare dishes and review the dishes placing more pressure on the kitchen. Improving staff retention was a broader goal.


## Business insights

<img width="1257" height="706" alt="informe ejecutivo" src="https://github.com/user-attachments/assets/0e58e46e-1835-4bcb-959f-ba478b0e3c1f" />

- Customers spent approximately **€20 per ticket** on average.
- **Sunday lunchtime** was the busiest period.
- **Takeaway accounted for approximately 45% of revenue.** This suggests delivery is worth investigating.

## Identifying dishes to promote or review

<img width="1256" height="708" alt="analisis" src="https://github.com/user-attachments/assets/0fd29106-6dd9-43b1-a142-24bf1ad64b68" />

I plotted dishes on a scatter chart using two measures:

- **Popularity:** based on the number of units sold.
- **Preparation difficulty:** a score from 1 to 5 based on whether a dish is made to order (40%), active preparation time (30%), number of steps (15%) and number of staff required (15%). This is a structured operational estimate rather than a timed measurement. 5 = hard to make 1 = easy to make

Popular dishes that were comparatively easy to make were candidates for promotion. Less popular dishes that were difficult to make were candidates for review.

## Changes in the Menu

<img width="1260" height="702" alt="cmabios" src="https://github.com/user-attachments/assets/ad196ad5-24d1-48dc-8c4f-9ca16d49da51" />

| Action | Decisions |
| --- | --- |
| Promote | Feature suitable dishes in a set menu, make them more visible on the menu and price at a more competitive price point. |
| Demote | Removed from menu or price at a higher price point. |

## Measuring the outcome

<img width="1257" height="705" alt="kpi" src="https://github.com/user-attachments/assets/dbd96ab6-feb5-46c2-b26b-3b2b21179b0f" />

I defined two indicators to compare the periods before and after the menu changes:

1. **Dish concentration:** The Herfindahl–Hirschman Index (HHI) measures how concentrated dish sales are. It increased by 4.6%, indicating that sales became more concentrated among fewer dishes.
2. **Estimated workload per €100 of sales:** I calculated a workload index as units sold × preparation difficulty, then divided it by sales value to compare periods with different revenue levels. This index decreased by 5.5% per €100 of customer spending.

These are observed before-and-after differences. Other changes in demand, prices or customer mix could have contributed to them.

## Limitations and next steps

- The analysis does not include ingredient costs or dish-level profit margins. These should be checked before changing prices or removing dishes.
- Difficulty scores are estimates. Timing preparation and checking the scores with kitchen staff would improve the workload measure.
- The data cover selected months rather than a full year, so seasonality may affect the comparison.

## Tools

- **Excel:** data cleaning and preparation.
- **Power BI:** data modelling, measures, visualisation and dashboard.
