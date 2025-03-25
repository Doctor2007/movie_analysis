# Movie Analysis

## Overview
This repository contains an analysis of movie ratings to determine the most impactful factors influencing ratings, compare IMDb and Metacritic scores, and assess how movie ratings have evolved over time.

## Research Questions
- What factors have the greatest impact on movie ratings?
- How do IMDb scores correlate with Metacritic scores?
- How have movie ratings evolved over time?

## Hypotheses
- The most impactful metrics on movie ratings are runtime, genre, and revenue.
- Action films receive higher average ratings than other genres.
- IMDb ratings are less varied than Metacritic ratings.
- The average movie ratings have declined over time, and the gap between critic and audience ratings has widened.

## Data and Sampling Plan
- Only movies with complete data for the relevant metrics are included.
- A proportionate number of movies by genre and time period are sampled.
- IMDb and Metacritic scores are standardized to the same scale for comparison.

## Analysis Plan
- **Impact on Ratings:** Multiple regression modeling with backward selection, using standardized beta coefficients to determine the most significant predictors.
- **IMDb vs. Metacritic:** Comparison of distributions using box plots, histograms, and paired t-tests.
- **Ratings Over Time:** Statistical tests on central tendencies (mean, median, mode) and t-tests for significance.

## Interpretation of Results
- A statistically significant and meaningfully large effect size for a given metric supports that it is **most impactful**.
- A strong correlation between IMDb and Metacritic suggests similar evaluative standards, while a weak correlation suggests differing criteria.
- Changes in measures of central tendencies over time indicate evolving rating trends.

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

