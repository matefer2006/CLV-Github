Goal:
Have a clear way of estimating future purchase amount depending on historical information.

Filters applied:
Removed 1% top Revenue or Time Between Orders quantiles (outliers).
Accounts that bought 2 or more times.

Definitions:
Frequency: How many purchases – Different order dates
Recency: Spread between the Account's last and first purchase
T: Spread between the model’s run date (usually today) and the Account's first purchase
Monetary value: Average order value - Grouped by order date, NOT order number

Technical explanation, two models: 
BG/NBD model - used to predict “Expected Number of Purchases” (any period from 0-12 months in the future).
Gamma/Gamma model - used to predict “Customer lifetime value” (how much money is it going to generate in the previously selected period).

Usage:
- Segmentation: depending on how much value accounts are expected to generate.
- Revenue or number of purchases prediction: at a accounts level or overall.
- Track metric’s distribution throughout time (Frequency, Recency and Monetary value).
