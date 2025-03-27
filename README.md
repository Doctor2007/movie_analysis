# Movie Analysis: What Makes a Great Movie?

## Overview
This repository contains an analysis of movie ratings to determine the most impactful factors influencing ratings, compare IMDb and Metacritic scores, and assess how movie ratings have evolved over time.

## Research Questions and Hypotheses

### 1. Do IMDB scores differ from Metacritic?
**Hypothesis:**
- H0: There is no difference in variation between IMDB ratings and Metacritic ratings.
- H1: IMDB ratings are more varied than Metacritic ratings.

**Sampling Plan:**
- Sample all movies that have a rating from both platforms.
- Convert metacritic ratings scale to IMBD rating scale (×10)

**Analysis Plan:**
- Compare measures of central tendencies (mean, median, mode)
- Compare distributions of ratings (density plot, scatter plot)
- Test for significant difference in mean (two-sided t-test)

**Test Sensitivity Rationale:**
- Test at 5% significance, as it best balances the risk of making type 1 and type 2 errors (false positive/negative) whilst providing a widely accepted level of accuracy

**Interpretation of Outcomes:**
- ACCEPT HYPOTHESIS (H1): Statistically significant p-value (<0.05) - We will use Metacritic scores as an alternative unit of measurement of movie rating.
- REJECT HYPOTHESIS (H1): Not statistically significant p-value (>0.05) - We will NOT use Meta Score as it isn't significantly different from IMDB score.

**Theory Being Tested:**
- Movie rating platforms tend to rate the same movies similarly.

### 2. How have movie ratings for both platforms changed in relation to release date?
**Hypothesis:**
- The difference between critic ratings (Metacritic) and audience ratings (IMDb) has widened over time

**Sampling Plan:**
- Do not use items with missing values for any of these metrics
- Have a proportionate number of movies from each time period (by decade for example)

**Analysis Plan:**
- Compare measures of central tendencies (mean, median, mode)
- Test for significant difference in mean (t-test)

**Test Sensitivity Rationale:**
- Test at 5% significance, as it best balances the risk of making type 1 and type 2 errors (false positive/negative) whilst providing a widely accepted level of accuracy

**Interpretation of Outcomes:**
- ACCEPT HYPOTHESIS: Statistically significant p-value (<0.05) - Measures of central tendencies across time have changed - movie ratings have changed
- REJECT HYPOTHESIS: Not statistically significant p-value (>0.05) - Measures of central tendencies across time have not changed - movie ratings have not changed

**Theory Being Tested:**
- Movie ratings have become higher over time

### 3. What variable is the best predictor of movie rating?
**Hypothesis:**
- Runtime is the most accurate predictor of movie ratings.
- We chose this hypothesis because it is specific, falsifiable, and testable.

**Sampling Plan:**
- Exclude items with missing values for any variables being used in the model.
- Use as many items in the data set as we can, so the model represents as much data.

**Analysis Plan:**
- Multiple regression modelling (runtime, certificate)
- Control for certain variables (revenue, year released)
- Check partial correlation coefficients and corresponding p-values, for runtime, certificate etc.

**Test Sensitivity Rationale:**
- A statistically significant and meaningfully large effect size for a given variable supports that it is an accurate predictor of rating.

**Interpretation of Outcomes:**
- ACCEPT HYPOTHESIS: If the selected variables return significantly different p-values we say that there is a clear relationship between those variables and movie ratings
- REJECT HYPOTHESIS: If all the variables return similar p-values we could say that there is no clear relationship between any variables and movie rating.

**Theory Being Tested:**
- Nothing can predict the rating of a movie. We live in chaos.

## Installation and Usage
To clone this repository, use the following command:
```sh
git clone https://github.com/Doctor2007/movie_analysis.git
```

Navigate into the project directory:
```sh
cd movie_analysis
```

Install the required dependencies:
```sh
pip install -r requirements.txt
```

## Libraries Used
This analysis utilizes the following Python libraries:
```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np
import scipy.stats as sp
```

## Repository Link
[GitHub Repository](https://github.com/Doctor2007/movie_analysis)

## Author
**Doctor2007**