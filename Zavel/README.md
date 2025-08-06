# House Price Prediction - Pakistan Real Estate

This project uses **machine learning models** to predict house prices based on property features in Pakistan. It leverages ensemble and tree-based regressors to provide accurate pricing estimates.

---

## Overview

This file includes two models:

1. **Random Forest Regressor**  
2. **Decision Tree Regressor**

Both models are trained on real estate data using key features such as area (in marla), number of bedrooms/bathrooms, location, and more.

---

## Why Random Forest?

Random Forest is a powerful **ensemble learning** technique that builds multiple decision trees and averages their predictions. It helps reduce overfitting and generally provides more robust and accurate predictions than a single decision tree.

---

## Dataset & Preprocessing

The dataset includes real estate listings with the following columns:
- `price`
- `area`
- `bedrooms`
- `bathrooms`
- `location`
- `floors`
- `parking_spaces`
- `furnished`

### Key Preprocessing Steps:
- Converted price strings (e.g., "PKR 2 Crore") into numeric PKR values.
- Converted area units (e.g., kanal, marla, sq ft) into **marla**.
- Extracted neighborhood information from the `location`.
- Encoded neighborhoods as numerical codes.
- Filled missing values in selected features.

---

## Features Used for Modeling

```text
area_marla
bedrooms
bathrooms
neighborhood_code
parking_spaces
furnished
