# The Impact of Major Commodities on Crude Oil Prices (2000–2020)

## Overview

In this project, I analyzed the impact of major commodities on crude oil prices from 2000 to 2020 using a dataset comprising 17 variables and 246 monthly observations. The study employed various statistical modeling techniques, including:

- Best subset selection
- Forward and backward stepwise regression
- Lasso regularization
- Cross-validation and model comparison

The results highlight the significant influence of certain commodities, especially energy-related ones, on crude oil prices. The analysis also explored the effects of major global events such as the 2008 financial crisis and the COVID-19 pandemic.

---

## Methods

- **Variable selection** via `regsubsets()` (leaps package)
- **Regularization** with Lasso (`glmnet`)
- **Cross-validation** to compare models
- **Model diagnostics**: residuals, leverage, collinearity (VIF)
- **Prediction** based on centered variables
- **Interpretation** of coefficients with real economic meaning

---

## Main Findings

- Energy commodities like **coal** and **natural gas** have the strongest linear relationship with crude oil prices.
- The **2008 financial crisis** had a measurable effect, confirmed through the `Post_Crisis` variable.
- A **log-transformation** of crude oil prices improved model diagnostics and interpretability.
- The best model explained **over 90%** of the variance in crude oil prices.

---

## Dataset Source

Data was retrieved from the [World Bank](https://www.worldbank.org/) and includes monthly commodity prices for:

- Energy (Coal, Natural Gas)
- Metals (Aluminum, Lead, Zinc, Gold)
- Agricultural (Banana, Cocoa, Cotton, Coconut Oil, Wheat, etc.)

---

##  Notes

- The `.Rmd` file can be rendered in RStudio with `knitr` or `rmarkdown::render()`.
---




