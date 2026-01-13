# Arabica Coffee Sensory Analysis and Predictive Modeling

## Overview
This project presents an end to end data analysis of Arabica coffee cupping ratings based on a public dataset curated according to the Specialty Coffee Association (SCA) protocol.  
The analysis explores how sensory attributes and technical factors contribute to subjective cup quality scores, with a focus on identifying key drivers and potential hidden effects.

## Dataset
The dataset contains 1,318 Arabica coffee cupping records collected between 2004 and 2018.  
Each record represents a single cupping evaluation and includes:
- Sensory scores such as Aroma, Flavor, Acidity, Aftertaste, Body, Balance and others
- The subjective overall score Cupper Points
- Technical attributes including country of origin, processing method, altitude and moisture

The data is publicly available at:  
https://github.com/jldbc/coffee-quality-database

## Data Cleaning and Preprocessing
The preprocessing stage included:
- Removal of irrelevant or low-information features
- Handling missing values
- Standardization of measurement units
- Formatting and normalization of categorical variables
- Filtering categories with insufficient sample sizes to ensure statistical stability

## Exploratory Data Analysis
Exploratory analysis was conducted to:
- Examine score distributions and variability
- Identify outliers and low-variance features
- Compare sensory and subjective scoring behavior
- Explore differences across countries of origin and processing methods

This stage guided feature selection and informed the modeling strategy.

## Modeling Approach
Two modeling frameworks were applied:

### Linear Modeling
- Multiple linear regression using LASSO regularization
- Cross validation for model stability
- Assessment of the relative contribution of sensory and technical variables

### Non Linear Modeling
- Random Forest regression
- Identification of non linear interactions between features
- Feature importance analysis to evaluate indirect and latent effects

## Key Findings
- Sensory attributes explain most of the variance in Cupper Points
- Technical variables such as country of origin and processing method contribute only marginally in linear models
- Non linear models reveal interaction effects suggesting indirect influences, potentially reflecting a hidden reputation effect
- Flavor, Balance and Aftertaste emerge as the most influential predictors

## Conclusions
The results suggest that Arabica coffee quality scores are largely driven by sensory evaluation, but that technical information may influence scoring indirectly through non linear interactions.  
This highlights the potential presence of latent biases or reputation effects in subjective evaluation processes.

## Code
The full analysis was conducted in Python.  

⚠️ This notebook contains interactive outputs that are not rendered by GitHub.

👉 View the full notebook with outputs in Google Colab: 
https://colab.research.google.com/drive/16CdByTq605Ss6iPICJqUsbbr160OssIw

## Authors
Or Mager  
Inbar Babai
