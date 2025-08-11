# dairy_sales

7/25/2025

From Kaggle's Beata Faron, 'FMCG Daily Sals Data' (2022-2024).

I'll post below their 'about dataset' after I add my own comments and goals in using this dataset.

In preperation for my upcoming consulting business in a variety of things, I want to code fresh pieces of material, demonstrating prowess
in thoughtfulness, analysis, and order. 

So, this looks like a promising dataset with over 190k entries over three years - we should be able to do a lot with it. Unfortunately the data is syntheic, yet the process of observing whatever remains the same and should be more than adequate in demonstating my abilities to potential clients. However, let's make a formal data problem of sorts to motivate this type of thing (and serve as a paradigm for any other organization with data really):

A small overworked grocery store in Poland has steady sales but isn’t sure how well they’re performing over time. With years of sales data sitting unused, they want to understand what’s working, what’s not, and where to focus efforts—whether that’s boosting juice sales or cutting underperforming items—to grow profitability.

## From Kaggle:

About Dataset
This synthetic dataset simulates daily-level FMCG sales transactions for three consecutive years (2022, 2023, 2024), designed for practicing time series forecasting, demand planning, and machine learning in realistic business conditions.

Inspired by real-world scenarios (e.g. Nestlé, Unilever, P&G), it includes:

Product hierarchy: SKU → Brand → Segment → Category
Sales channels: Retail / Discount / E-commerce
Regions: Central, North, and South (Poland)
Daily sales quantities, prices, promotions, stock, delivery lag (lead time)
Pack types: Single / Multipack / Carton
Seasonality and product introductions:
New SKUs are introduced in 2024 only
Prices gradually increase over the years
Possible Use Cases

Weekly sales forecasting
Promotion effect analysis
Seasonality and trend modeling
New product forecasting (cold start)
Feature engineering for ML models
Created by: Beata Faron
LinkedIn profile
Data Scientist working on demand forecasting, NLP, and business-oriented ML.

## Findings

After a bit of cleaning and engineering (such as by seperating out dates into components like day of the month), we went through all the data, trying to observe each feature's nature (categorical vs. numerical) & distribution (such as mean and standard deviation) as well as numerous bi or tri-feature relationships, focusing obviously on our target of price.

Action wise, we can suggest the following to the grocery store (recall that the data is synthetic and I highly doubt one would find any of these results, let alone all of them, in reality):

1) Consumers seem to not care about the price of whatever they're buying, so you might as well hike up the prices (from this data we can safely suggest even up to 9 zloty per (Polish dollars) per item) and make more money per item.

2) All products are not purchased equally, so try to focus on buying more yogurt and not as much juice (the most and least popular correspondingly).
b) Similarily, so too with brands. Ex.  Snack Brand 2 is at least 3 times as popular as Snack Brand 3 so make sure to have ample amounts of the former and not focus as much on the later.

3) Sales are cyclical according to the calendar quarter, with the least amount of sales in the first quarter and steadily increasing by over 40% once the fourth quarter comes along. So, be much more stocked as the calendar year goes by aand not sad about a sudden 'drop' in sales once the first quarter arrives.

4) When it comes to most other factors, such as the channel of acquisition or regional differences, they really don't affect sales. So, your nephew might have made an Oscar-winning online advertisement for people in Southern Poland - but the data shows they don't spend any more than the other regions so there's no justification (save not getting yelled at by your sister) for letting him spend a million dollars on his idea.