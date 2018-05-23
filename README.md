---
title: "ThresholdFuzzyRoughQuickReduct"
author: "Javad Rahimipour Anaraki"
date: '23/05/18'
---

## Use case
To determine the most important features using an improved version of Fuzzy-Rough QuickReduct algorithm as described in [Improving fuzzy-rough quick reduct for feature selection](https://ieeexplore.ieee.org/document/5955425/) By Javad Rahimipour Anaraki and Mahdi Eftekhari

More info can be found in [Novel Improvements on the Fuzzy-Rough QuickReduct Algorithm](https://www.jstage.jst.go.jp/article/transinf/E98.D/2/E98.D_2014EDL8099/_article)

## Compile
This code can be run using MATLAB R2006a and above

## Run
To run the code, open `main.m` and choose a dataset to apply the method to. At first, the overall dependency degree is calculated using `dependency.m`. Then, indisernible objects are determined and returned to `main.m`. Finally, feature are selected if they have the best dependecy degree among all. This process stops if `(totalDD - max(maxDD(2, :))) * r < 1` or maximum dependency degree does not improve with adding extra features.

All datasets are stored in *Data* folder and originally adopted from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)

## Note
Datasets should have no column and/or row names, and the class values should be all numeric
