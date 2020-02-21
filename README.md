# Predicting Geospatial Affluence With Yelp Data

### Project Authors
- Pablo Rivera | <u>[LinkedIn](https://www.linkedin.com/in/pabrivera/)</u>
- Elizabeth Jafek | <u>[LinkedIn](https://www.linkedin.com/in/elizabeth-jafek/)</u>
- Libin Huang | <u>[LinkedIn](https://www.linkedin.com/in/libinh/)</u>

---

### Table of contents
- <u>[Problem Statement](#Problem-Statement-and-Key-Objective)</u>
- <u>[Executive Summary](#Executive-Summary)</u>
- <u>[Findings](#Findings)</u>
- <u>[Conclusion and Recommendations](#Conclusion_and_Recommendations)</u>

---

### Problem Statement and Key Objective
<b> Problem Statement </b>
- Traditional methods estimate geospatial wealth via income or unemployment rates

- However these data sources are not always updated frequently enough or may not provide sufficient granular data for the agile needs of disaster response agencies

<b> Key Objective </b>
- Build a model that will take zip codes or location as input and will leverage frequently updated commercial data to estimate geospatial affluence with high accuracy

---


### Executive Summary
- Yelp Dollar sign ($) data alone is not a strong predictor of geospatial affluence
      - Correlation of Yelp Dollar Sign to Median Income is 0.11
- Challenges observed: limited venue/business/service representation in low affluence or low population areas, non-residents providing yelp reviews
- However by augmenting Yelp Dollar Sign data with median home value with price ratings, population, and classifying cheap and expensive restaurants, the train/test scores improved
- Ultimately we were able to achieve our key objective of accepting a location as input and estimating with 65.5% accuracy the location’s affluence

---

### Conclusion and Recommendations
- Do not rely solely on Yelp price level data to predict affluence
- Continue building robustness of model with scheduled periodic Yelp Data updates to continue training model and improving accuracy
- Consider purchase of Commercial Grade Yelp API access in order to streamline data extraction
- Expand functionality and improve user-experience by building front-end with Flask or similar tool
