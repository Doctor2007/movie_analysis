# Movie Analysis: What Makes a Great Movie?

## Project Overview
This project analyses IMDb's top 1000 movies dataset to understand what factors contribute to high movie ratings and how audience perceptions compare to critic evaluations.

## Research Questions
1. **Do IMDb scores differ from Metacritic?** - Explored differences between audience and critic ratings
2. **How have movie ratings changed over time?** - Analyzed rating trends across different decades
3. **What factors best predict movie ratings?** - Identified variables with strongest correlation to high ratings

## Key Findings
- **Audience vs. Critic Divergence**: Statistical testing (p<0.05) confirmed significant differences between IMDb ratings and Metacritic scores
- **Rating Trends**: IMDb ratings are more stable over time while Metacritic scores show greater fluctuation
- **Predictive Factors**: Runtime, director experience, and release year have small but significant effects on ratings
- **Limited Explanatory Power**: Our multiple regression model explains ~14% of rating variance, suggesting movie success is influenced by many complex factors

## Methodology
- Data cleaning and preparation
- Statistical tests including t-tests
- Single and multiple linear regression
- Feature engineering (certificate categorisation, star power metrics)
- Time series analysis
- Data visualisation (density plots, violin plots, regression plots)

## Technologies Used
- Python (pandas, seaborn, matplotlib, numpy, scipy.stats, statsmodels)

## Getting Started
```bash
git clone https://github.com/Doctor2007/movie_analysis.git
cd movie_analysis
pip install -r requirements.txt
jupyter notebook main.ipynb
```