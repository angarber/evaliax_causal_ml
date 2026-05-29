# Causal ML Tutorial Series (EvaliaX v1)

This repository contains a set of tutorials on **causal machine learning using Causal Forests**, applied to a simulated subsidy allocation dataset.

The goal is to explore heterogeneous treatment effects and interpretability techniques in causal inference using modern machine learning tools.

---

## Project Structure

```
causalml_evaliax_v1/
│
├── data/
│   └── simulated_subsidy_dataset.csv
│
├── notebooks/
│   ├── v1_causal_forest_tutorial.ipynb
│   ├── v2_xai_causal_forest_tutorial.ipynb
│   └── v3_iai_causal_forest_tutorial.ipynb
│
├── assets/
│   └── logo_evaliax.png
│
└── README.md
```

---

## Objectives

- Estimate heterogeneous treatment effects (CATEs) using Causal Forests
- Analyze treatment effect variation across firms
- Compare different explainability approaches:
  - Variable importance
  - Best Linear Projection (BLP)
  - Rashomon perspective on model multiplicity
- Improve interpretability of causal machine learning models

---

## Key Concepts

### Causal Forest
An ensemble method for estimating Conditional Average Treatment Effects (CATEs) in high-dimensional settings with flexible, nonparametric heterogeneity.

### Best Linear Projection (BLP)

The BLP approximates heterogeneous treatment effects using a linear projection:

$$
\tau(X) \approx X' \beta
$$

This provides a simple, interpretable summary of how covariates are associated with treatment effect variation.

### Rashomon Effect
Multiple models can achieve similar predictive performance while implying different structural explanations. This highlights that there may be several equally valid representations of heterogeneity.

---

##  Dataset

The dataset is synthetically generated and simulates firm-level responses to a subsidy program. It is designed for educational and methodological purposes.

---

##  Requirements

Typical Python dependencies include:

- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn
- econml / causalml

---

##  Notebooks

- **v1_causal_forest_tutorial.ipynb** → Baseline causal forest estimation
- **v2_xai_causal_forest_tutorial.ipynb** → Explainability (BLP, importance, interpretation)
- **v3_iai_causal_forest_tutorial.ipynb** → Advanced interpretability analysis

---

##  Assets

Includes project logo and auxiliary visual materials used in notebooks and presentation figures.

---

##  Author

EvaliaX Research Team

---

##  License

This project is for research and educational purposes only.
