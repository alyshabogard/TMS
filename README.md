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
