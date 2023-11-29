# Market Basket Analysis with Apriori Algorithm

## Introduction and Objective
This repository contains a Python ipynb file for performing Market Basket Analysis using the Apriori algorithm. Libraries like pandas, seaborn, and matplotlib.pylot were 
equally used. The analysis was performed on a grocery dataset to understand the association of the various products.

## High-Level Steps
  - **Data Loading and preparation:**
  - Import the necessary libraries
  - Load the grocery sales data and performed necessary data cleaning.
  - Convert 'Member_number' to a string and 'Date' to datetime format.
  - converted the 'itenDescription' to a snake case

    **Exploratory data analysis(EDA)**
  - Product category distribution using a pie chart and a barplot
  - Frequency distribution of itens
  - Distribution of number of items per transaction using a histplot

## Apriori algorithm
  - Importing the required libraries
  - from mlxtend.frequent_patterns import apriori
  - from mlxtend.frequent_patterns import apriori, association_rules

- **Unique identifier:**
  - Create a new column that combines the 'Member_number' and 'Date' into a single unique identifier.

- **Cross-Tabulation (Basket Creation):**
   - Create a cross-tabulation ('basket') to represent the frequency of items in each unique transaction.
   - Create a binary-encoded DataFrame

- **Apriori Algorithm and Association Rules:**
  - Apply the Apriori algorithm to generate frequently bought itemsets, using min_support as 0.005
  - Use association rules, focusing on Zhang's metric for evaluation.

- **Heatmap Visualization:**
  - Represent product associations through the use of a heatmap.
  - Interpret the heatmap to understand frequent itemsets.

- **Positive Association Visualization:**
  - Investigate pairs exhibiting positive Zhang's metric to emphasize favorable associations.

## Visualization
- Utilize heatmaps for clear and intuitive visualization of product associations.
- Explore positive associations to understand which products complement each other.

## Insights
- Use Zhang's metric for a comprehensive evaluation of association rules.
- Interpret negative and positive values to understand anti-associations and strong positive relationships.

## Recommendations
- Wrote a code for generating recommendations using association rule
- Provided other recommendation

Feel free to explore the code and adapt it for your own datasets and analysis needs.
