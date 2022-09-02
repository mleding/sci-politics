# project-deliverables-mleding
project-deliverables-mleding created by GitHub Classroom


Executive Summary: This project uses county level social connectedness data from Facebook’s Data for Good
as well as demographic factors like race, education, income, and gender to predict voter
participation in the 2020 election. The work begins with sourcing and engineering data, in
particular, pivoting social connectedness data into distance buckets, normalizing into
proportions, and joining datasets together by county. Then, models are generated using OLS
linear regressions, Forward Step Feature Selection, Lasso Regression, General Linear Modelling,
and XGBoost with Randomized Search parameter tuning. Models are compared by using root
MSE scores to select for the most effective model. Finally, comparisons are made between
models containing Social Connectedness Data as well as those without it to examine whether
social connectedness has any predictive power towards vote participation. 

------


Hi Visitors!

This repository has the files as well as my code for the project. BIG NOTE, github won't let me upload data files greater than 100MB. I was able
to get around most of it by compressing the files. There is one data files that needs to be downloaded from the source.

This repository contains:

annotated_project_report.pdf: this is documentation and analysis of project. Please start here.

project_code.ipynb: this is a jupyter notebook file containing all my code. This contains 617 lines of code.

County_CVAP.csv.zip: this is a zip file for the county citizen voter age population data. Git won't let me upload files over 100mb so this needs to be unzipped and 
  named County_CVAP.csv. From https://www.census.gov/programs-surveys/decennial-census/about/voting-rights/cvap.html

Poverty.csv: this is a zip file containing poverty data. Source: https://www.ers.usda.gov/data-products/county-level-data-sets/

county_county.tsv.zip: this is the facebook SCI data that pairs counties and tallies facebook connections between them. Again, it is a zip file 
  that needs to be unzipped and renamed to county_county.tsv before it can be run. Source: https://dataforgood.facebook.com/dfg/docs/methodology-social-connectedness-index


demographic.csv.zip: this contains demographic data on race and gender. This needs to be unzipped and renamed demographic.csv. 
  From https://www.census.gov/data/tables/time-series/demo/popest/2010s-counties-detail.html

education.csv: this contains education data. Source: https://www.ers.usda.gov/data-products/county-level-data-sets/

election.csv: this contains data on 2020 presidential election.
  Source: https://github.com/tonmcg/US_County_Level_Election_Results_08-20/blob/f9b5f335ad1c66a7eba681539db49eec0c22787b/2020_US_County_Level_Presidential_Results.csv

unemployment.csv: this contains unemployment data as well as income level. Source: https://www.ers.usda.gov/data-products/county-level-data-sets/

ADDITIONAL:
Please go to https://www.nber.org/research/data/county-distance-database and download the 2010 county distance csv file and name it countydistancemiles.csv. 
I could not upload this file on github, as even compressed, it was too large. 
