

# An Analysis of Sovereign Credit Risk

![alt text](https://github.com/anaulianova/Capstone_Project/blob/master/images/image.jpg)

## Project Overview
Sovereign risk ratings are used by investors to gain insight and assess the level of risk associated with the purchase of sovereign debt. Countries with a higher rating accordingly have low risk, and thus the purchase of sovereign bonds issues by such countries are marked as a low-yield, low-risk investment. 

However, as the credit rating lowers and the risk of default rises, so does the yield, providing a middle ground for opportunity for higher-yields, given an investors appetite for a higher risk. Accordingly, being able to understand what factors may lead a country to default on its responsibilities is crucial to investors to protect their assets, while capturing opportunities for greater return in emerging markets. 

Thus, I have attempted to examine the relationships between a wide variety of  national indicators, the majority of which were sourced from data assembled by the World Bank, in order to build a predictive model & gain a clearer understanding of the importance of various features to a country’s credit worthiness. 

## Data Sources

* World Bank Data Bank: https://data.worldbank.org/indicator?tab=all 
* UN Trade Statistics: https://unstats.un.org/unsd/tradekb/knowledgebase/country-code
* Wikirating - List of countries by credit rating: https://www.wikirating.org/wiki/List_of_countries_by_credit_rating
* Trading Economics: https://tradingeconomics.com/country-list/rating
* Transparency International: https://www.transparency.org/en/cpi/2020 


## Methodology

-	Source, gather and webscrape data to create an original dataset
-	Clean and prep the data 
-	Perform Exploratory Data Analysis, with visualizations to better understand the different features of the dataset
-	Use a Support Vector Machine to model the data

## Findings


The Exploratory Data Analysis revealed a strong relationship between Credit Rating and the several variables, which highlights features that are of interest to the objective of this analysis. 
### 1. Credit Rating & Income Group


Unsurprisingly, the wealth of a state is very strongly affected by where that state will rank amongst the credit rating categories, with wealthier nations concentrating on the top half of the Credit Rating categories, and lower income countries concentration on the bottom half. 

### 2. Credit Rating and Region

The distribution of Credit Rating classes by region is relatively normally distributed (with some skewness in one direction or another depending on the region). By this spread, European and Asian countries appear to generally have a higher rating than other regions. 
In terms of opportunity, Latin American presents an interesting case with its countries primarily concentrating around the center of the credit rating spectrum, yet still with many counting in the upper half, showing a positive skew towards a better credit score. 


Nonetheless, the complexity & shortness of the dataset has to an inconclusive result, despite exploring the use of various kernels including Polynomial, Sygmoid, RBF and linear. 

The findings are as follows: 

### Polynomial: 
Test Accuracy of 18.42%
### Sygmoid: 

### RBF: 
Test Accuracy of 23.68%
#Linear: 
inconclusive due to excessive running time (over 6 hours with no result)
# Recommendations
Though the model still lacks data to make a conclusive prediction across the board, when tackling higher risk markets, investors should focus on the following:
- Looking at the strong relationship between Credit Rating and such variables as Income Group and Ease of Doing Business Index, investors should monitor the business environment in emerging markets, specifically focusing on the presence of a growing number of entrepreneurship and small & medium businesses. Such factors could provide early indicators of an improving economy.

- Monitor news cycles of the country, specifically focusing on the presence of any corruption scandals, given the strong positive relationship between corruption and poor credit rating. 

- Consider the region of interest alongside considerations for risk appetite.

## Future Research
> Continue to test features to add to the model including:
- Freedom Scores
- Presence of internal or regional conflict
- Primary national industries
- Level of natural resources & type
> Incorporate Time Series aspect to increase the length of the dataset & explore the time variable’s effect on different countries’ sovereign risk
> Zoom in on historic cases where countries have defaulted on their debt to identify common patterns leading up.
