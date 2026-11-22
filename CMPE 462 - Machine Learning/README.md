# CMPE 462 — Machine Learning

**Course Project (Fall 2026): Backpack Inventory**

## About

Backpack Inventory is a semester-long group project built around a multimodal school-item classification dataset that the class collects itself. Every group contributes samples of the same five classes (pencil, pen, eraser, notebook, and sharpener) to one shared dataset, which all groups then use for a supervised and an unsupervised task. Each sample combines a photo of the item, a recording of it being dropped on a desk, a one-sentence description, and measured attributes such as length, weight, color, material, and price. The dataset deliberately mixes real samples with synthetic ones, produced by generative models, fitted distributions, or data augmentation.

## What students were asked to do

- **Data Contribution:** Collect at least 50 real samples from at least 10 different items and add at least 100 synthetic samples for each class, following a strict Parquet schema and privacy rules. Submissions must pass a validation script and a manual audit, and include a data card describing how the samples were collected and generated.
- **Task 1 — Supervised Learning:** Extract fixed-length features from every modality (without deep models for images), fuse them, and analyze class similarity, outliers, and dataset difficulty. Train and compare linear vs. nonlinear and discriminative vs. generative classifiers, with at least one implemented from scratch, and combine them in an ensemble. Evaluate with modality ablation, hybrid real/synthetic training ratios, error analysis, calibration, and feature interpretation.
- **Task 2 — Unsupervised Learning:** Explore intrinsic dimensionality with PCA and retrain on the reduced features, then cluster the data and test whether clusters reflect item class, material, or provenance. Compare structure across modalities, design a detector for fake image–audio or image–text pairs, build an unsupervised outlier detection framework, and use unlabelled data to approach Task 1 accuracy with only *k* labelled samples per class.

Grading is split between the data contribution (20%), the Task 1 and Task 2 reports (30%), and an oral evaluation (50%).

## Context

This is the main machine learning course project: it covers the full pipeline from data collection and quality control through feature engineering, classification, model evaluation, dimensionality reduction, clustering, outlier detection, and semi-supervised learning. Because students work with a dataset they built themselves, it also raises practical questions that textbook datasets avoid, such as group-level bias, item-level data leakage, and whether models trained on synthetic data transfer to real data.

The full project description is in [`cmpe462_fall26_project_backpack_inventory.pdf`](cmpe462_fall26_project_backpack_inventory.pdf).
