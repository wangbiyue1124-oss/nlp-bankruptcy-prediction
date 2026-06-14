# NLP-Based Bankruptcy Prediction

Predicting corporate bankruptcy risk using NLP models applied to SEC 10-K filings and NYT financial news.

## Overview

This project applies and compares multiple NLP sentiment analysis models to financial text data, evaluating their effectiveness in identifying bankruptcy risk signals. The goal is to support credit risk assessment using publicly available financial disclosures.

## Models Compared

| Model | Accuracy |
|-------|----------|
| FinBERT | 73% |
| RoBERTa (Zero-shot) | — |
| VADER | 33% |
| Zero-shot Classifier | — |

FinBERT significantly outperformed the lexicon-based VADER approach, demonstrating the advantage of domain-specific pre-trained models for financial text.

## Data Sources

- **SEC 10-K filings** — annual financial reports from public companies
- **NYT financial news articles** — external news signals around filing periods

## Tech Stack

Python · pandas · scikit-learn · HuggingFace Transformers · VADER · FinBERT · RoBERTa

## Key Findings

- Domain-specific models (FinBERT) outperform general-purpose sentiment tools (VADER) by ~40 percentage points on financial text
- SEC 10-K language contains meaningful risk signals detectable through NLP
- News sentiment provides complementary signals to formal disclosure language

## About

Academic project — MS in Data Science, Saint Peter's University (2026)
