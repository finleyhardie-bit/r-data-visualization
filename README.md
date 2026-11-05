# R: Data Visualization & Machine Learning

**Finley Hardie** · University of Denver, Daniels College of Business
Portfolio site: **[finleyhardie-bit.github.io](https://finleyhardie-bit.github.io)**

R and Quarto work from INFO 3200 (Spring 2026): two full case studies, machine-learning assignments, visualization work and a class presentation. Each folder has the Quarto (`.qmd`) source. The two case studies can also be read as finished reports on my site.

| Folder | What's inside |
|---|---|
| [`case-study-2-loan-default/`](case-study-2-loan-default) | **Featured.** Predicting loan default risk with four models |
| [`case-study-1-ecommerce/`](case-study-1-ecommerce) | **Featured.** E-commerce revenue, customer segments and seasonality |
| [`machine-learning/`](machine-learning) | Decision trees, kNN, naive Bayes, ROC and model evaluation |
| [`visualization/`](visualization) | ggplot2 chart types and a Denver crime map |
| [`time-series-presentation/`](time-series-presentation) | Slides I co-presented to the class |

---

## Case Study 2: Predicting loan default risk
**[Read the report](https://finleyhardie-bit.github.io/reports/loan-default-risk.html)** · Source: [`loan-default-risk.qmd`](case-study-2-loan-default/loan-default-risk.qmd)

A fictional lender wants to catch risky borrowers. Of 3,357 complete applications, 27.5% were bad risks, so approving everyone is already 72.5% accurate.

- Compared a baseline, a decision tree, logistic regression and two random forests, plus three regression models for loan size.
- **Logistic regression generalized best: 74.3% test accuracy, with only a 1.7-point train/test gap.** The random forests scored 96%+ on training data but about 73% on new data (overfitting).
- Prior default history was the strongest predictor in every model. I recommended treating it as a near-disqualifying flag and adding income tiers and a debt-to-income cap to underwriting.
- Linear regression predicted loan size best (test R² 0.90, RMSE about 912).

**Tools:** tidymodels, rpart, ranger, ggplot2, gt

## Case Study 1: E-commerce analytics
**[Read the report](https://finleyhardie-bit.github.io/reports/ecommerce-analytics.html)** · Source: [`ecommerce-analytics.qmd`](case-study-1-ecommerce/ecommerce-analytics.qmd), [`ecommerce-dashboard.qmd`](case-study-1-ecommerce/ecommerce-dashboard.qmd)

Three years of transactions (2022–2024) from an online store with 1,000+ customers.

- Joined the transaction, customer and product tables and charted revenue by category, month and marketing channel.
- Segmented customers with k-means on recency, frequency and spend. The top segment averages about 8 orders and $11K each.
- A trend-plus-season regression puts July about $44.9K above January and February about $34.3K below it.
- Summarized everything in a Quarto dashboard.

## Machine learning → [`machine-learning/`](machine-learning)

| File | Topic |
|---|---|
| [`decision-trees.qmd`](machine-learning/decision-trees.qmd) | Classification and regression trees |
| [`knn-classification.qmd`](machine-learning/knn-classification.qmd) | k-nearest neighbors |
| [`naive-bayes-classification.qmd`](machine-learning/naive-bayes-classification.qmd) | Naive Bayes classification |
| [`roc-and-model-evaluation.qmd`](machine-learning/roc-and-model-evaluation.qmd) | ROC curves, precision-recall and probability calibration |

## Visualization → [`visualization/`](visualization)

| File | Topic |
|---|---|
| [`bar-and-line-charts.qmd`](visualization/bar-and-line-charts.qmd) | Sales by category and region, and monthly trends (Sample Superstore) |
| [`deviation-distribution-correlation.qmd`](visualization/deviation-distribution-correlation.qmd) | Histograms, density plots, a correlation matrix and a regression line |
| [`geospatial-mapping-denver-crime.qmd`](visualization/geospatial-mapping-denver-crime.qmd) | Static and interactive (Leaflet) maps of Denver crime data |

## Time series presentation → [`time-series-presentation/`](time-series-presentation)
**[View the slides](https://finleyhardie-bit.github.io/reports/time-series-presentation.html)**

Co-presented with Jack Callahan. It teaches trend, seasonality, noise and stationarity using the AirPassengers dataset.

---

*Datasets were provided by the course and aren't included here.*

**Tools:** R, Quarto, tidyverse, ggplot2, tidymodels, leaflet, sf
