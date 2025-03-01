# TMS Recruitment Curve Analysis 📊

## Overview
This repository contains a **MATLAB-based TMS recruitment curve analysis pipeline** designed to quantify **motor evoked potential (MEP) responses** pre and post **neuromodulation interventions**. 
The script:  
- Automates **data loading and preprocessing** for recruitment curves (RC) and maximal voluntary contraction (MVC) trials.  
- Computes **background noise correction** to ensure accurate MEP analysis.  
- Extracts key **neurophysiological biomarkers** such as **MEPmax, recruitment slope, and area under the curve (AUC)**.  
- Implements **Boltzmann curve fitting** to model **TMS excitability changes**.  
- Generates **visualizations** for pre/post **RC comparisons**.

## Features
✅ **Automated subject data import** (no manual file handling)  
✅ **Background noise subtraction** for precise **MEP quantification**  
✅ **Boltzmann curve fitting** to assess **recruitment slope & threshold**  
✅ **MEP intensity extraction** at 100%, 120%, 140% RMT  
✅ **Statistical output: AUC, peak slope, and MEPmax values**  
✅ **Batch processing for multi-subject analysis**  
✅ **Option to generate recruitment curve plots**  

## Dependencies
- **MATLAB R2020b or newer**  
- Required toolboxes:  
  - `Curve Fitting Toolbox` (for Boltzmann curve fitting)  
  - `Statistics and Machine Learning Toolbox`  

# Bayesian Analysis of TMS Recruitment Curve 📊

## Overview
This repository contains a **Bayesian statistical analysis pipeline** for investigating **motor evoked potential (MEP) responses** pre and post **AIH intervention** using **brms** in R. 
The script:  
- Implements **Bayesian regression modeling** to assess the impact of **time (pre vs. post-AIH) and background EMG (BG)** on log-transformed MEP amplitudes (**log_MEP**).  
- Uses **posterior distributions, credible intervals (CIs), and hypothesis testing** to quantify uncertainty.  
- Compares **two models (with and without BG)** using **LOO cross-validation** and **Bayesian R²**.  
- Performs **posterior predictive checks (PPCs)** to evaluate model fit.  

## Features
✅ **Bayesian mixed-effects regression** (random effect: subject ID)  
✅ **Custom prior distributions** for regularization  
✅ **Posterior predictive checks (PPCs) to validate model assumptions**  
✅ **Hypothesis testing via posterior probabilities**  
✅ **Model comparison using LOO-CV & Bayesian R²**  
✅ **Frequentist linear regression for validation**  

## Dependencies
- **R version 4.0+**
- Required packages: `brms`, `bayestestR`, `loo`, `ggplot2`, `tidyverse`, `lme4`  
