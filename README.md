# Estimating Heterogeneous Customer Responses to Pricing Interventions Using Uplift Modelling

An independent research project exploring the application of causal machine learning techniques to pricing decisions in maintenance service contracts.

---

## Overview

Traditional predictive models estimate whether a customer is likely to accept a service contract. However, they do not answer a more important decision-making question:

> **How would the probability of acceptance change if the same customer received a different pricing offer?**

This project investigates that question using uplift modelling and treatment-effect estimation. Rather than predicting customer behaviour alone, the study estimates the causal effect of a pricing intervention (discount) on contract acceptance for individual customers and customer segments.

The project was independently designed and implemented as a research-style study inspired by recent developments in Operations Management, Pricing Analytics, and Causal Machine Learning.

---

## Research Objectives

The project aims to:

- estimate heterogeneous customer responses to pricing interventions;
- compare predictive modelling with causal treatment-effect estimation;
- identify customer segments most responsive to discounts;
- demonstrate how causal machine learning can support data-driven pricing decisions.

---

## Methodology

The study consists of the following stages:

1. Generation of a synthetic dataset representing maintenance service contracts.
2. Exploratory data analysis.
3. Development of a predictive baseline using Logistic Regression.
4. Implementation of a T-Learner framework with Random Forest models.
5. Estimation of individual treatment effects (uplift).
6. Customer segmentation based on estimated uplift.
7. Visualisation and interpretation of experimental results.

---

## Dataset

The synthetic dataset contains operational, customer, and contract characteristics, including:

| Variable | Description |
|----------|-------------|
| `machine_age` | Age of the machine |
| `annual_usage` | Annual machine utilisation |
| `customer_size` | Customer segment (Small / Medium / Large) |
| `contract_duration` | Contract length (years) |
| `previous_failures` | Historical equipment failures |
| `discount` | Pricing intervention (treatment) |
| `accepted` | Customer acceptance of the contract |

---

## Main Findings

The experimental results demonstrate that:

- customer responses to pricing interventions are heterogeneous;
- treatment-effect estimation provides more informative insights than predictive modelling alone;
- smaller customers exhibit substantially higher estimated uplift than medium and large customers;
- uplift modelling enables targeted pricing strategies by identifying customers who are most likely to respond positively to discounts.

These findings illustrate the value of causal machine learning for operational decision support and pricing optimisation.

---

## Repository Structure

```
pricing-uplift-modelling/
│
├── report.pdf
├── uplift_modelling.ipynb
├── synthetic_dataset.csv
├── requirements.txt
└── README.md
```

---

## Technologies

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- Jupyter Notebook

---

## Reproducibility

After installing the required packages

```bash
pip install -r requirements.txt
```

open

```
uplift_modelling.ipynb
```

and execute all cells to reproduce the complete workflow, including:

- synthetic data generation;
- model training;
- treatment-effect estimation;
- visualisations;
- experimental results.

---

## Project Report

A detailed description of the methodology, experimental design, results, and discussion is available in:

**`report.pdf`**

---

## Author

**Anastasia Demidova**

Independent research project (2026)
