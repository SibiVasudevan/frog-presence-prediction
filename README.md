# Frog Presence Prediction

Minimal notebook solution for the **EY “Frog Challenge”** completed in the Analytics Practicum Course (MS Business Analytics & AI, UT Dallas, Spring 2025).

## Project brief

Predict frog presence vs absence in south‑eastern Australia (Nov 2017 – Nov 2019) using 14 monthly TerraClimate variables supplied through the Microsoft Planetary Computer. This satisfies the challenge objective of mapping habitat suitability as an early indicator of ecosystem health.

## Quick start

```bash
git clone https://github.com/SibiVasudevan/frog-presence-prediction.git
cd frog-presence-prediction
# open Group_11_Final_Model_Code.ipynb in Jupyter / Colab and Run‑All
```

The notebook fetches training and validation data, builds the model, and writes a predictions CSV.

## Workflow covered in the notebook

1. Load FrogID presence and synthetic non‑presence points
2. Harvest TerraClimate variables for each location
3. Optional feature engineering (rolling means, temp‑moisture interactions)
4. Train tuned XGBoost (baseline logistic & RBF‑SVM for comparison)
5. Evaluate (F1 ≈ 0.83)
6. Export predictions for the 2 000 validation points

