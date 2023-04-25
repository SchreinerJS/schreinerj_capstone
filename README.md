# Shape of the American Family

## Tableau Dashboard
Link:

## Table of Contents
* [Tableau Dashboard](#Tableau-dashboard)
* [Motivation](#motivation)
* [Questions](#questions)
* [Normalizing the Data](#normaling-the-data)
* [Issues and Limitations](#issues-and-limitations)
* [Technologies Used](#technologies-used)
* [Sources](#sources)
* [Conclusion](#conclusion)

## Motivation:
Inspired by the valiant efforts of my brother in years past as a single dad and the stories of single-mother coworkers and friends, an interest in the impact of WWII on the shape of the American family narrowed to a focus on the changing shape and trends of single-parent families and their incomes over time.

In review of the available data and many factors impacting single parents, I decided to review a several of these factors over time, including:

- Parenting structure (married couple, single parent, single mother, single father)
- Location (by state)
- Ethnicity (by state)
- Median and mean incomes
- [Marital structure (who are children living with)]
- [Number of earners in household]
- [Family size]

## Questions:
1) How has the shape of the American family changed over time?
2) What are some of the trends regarding the factors impacting single parent families and incomes over time?

## Normalizing the Data
Data was drawn primarily from U.S. Census Bureau Current Population Surveys Annual Social and Economic Supplements (CPS ASEC) Tables.  Additional single parent datasets were selected from datadiversitykids.org, which were calculated from Census Bureau American Community Survey (ACS) data.

Just as family structure and related factors have been changing, many Census variables and definitions have also been evolving to accommodate such changes.  There were also considerations of the need to make adjustments for current dollars.  Therefore the decision was made to utilize pre-tabulated which offered a variety of historical household, family, and income values calculated with the appropriate year-to-year adjustments.

Multiple dataframes were created from these Excel tables and cleaned in Python, building the long tables into wide tables to create headings of categorical values as well as removing footnotes, duplicated year values, transforming datatypes, and selecting only timeframes which had no missing data for one or more variables.  

## Issues and Limitations
The main issue was taking time to familarize oneself with the many Census Bureau variables and definitions present in each table, and determining which tool available was the better one to extract the needed data.  Choosing pre-tabulated data resolved the issue of normalizing over time, but brought with it the added factors of utilizing spreadsheet data rather than a database better designed for visualization and analysis.  Choosing to widen the tables may also not have been the better pathway in cleaning the tables for visualization in Tableau.  Finally, more tables were cleaned and prepared than time allowed for visualization, but these could provide opportunity for a deeper analysis into this subject in the future.

## Technologies Used
1) Excel - review and adjust column names
2) Python / Pandas - for exploration, normalizing and cleaning of the dataset
2) Tableau - for analysis and creation of an interactive dashboard
3) PowerPoint - for project introduction
4) GitHub - for version control

## Data Sources
To answer the above questions, the tables and datasets were pulled from the following sources for analysis:

1) Various Census Bureau Historical Households and Historical Household Income Tables
https://www.census.gov/data/tables/time-series/demo/families/families.html
https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-income-households.html

2) Various Census Bureau Family Households and Historical Family Income Tables
https://www.census.gov/data/tables/time-series/demo/families/households.html
https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-income-families.html

2) Early Warning Projects by ushmm.org. The dataset includes 2021-22 Statistical Risk Assessment for Mass Killing by Country.
https://earlywarningproject.ushmm.org/ranking-of-all-countries

3) Households that are single parent (count) by race/ethnicity
https://data.diversitydatakids.org/dataset/11001_2_c-households-that-are-single-parent--count--by-race-ethnicity
Calculated from American Community Survey Summary Files

4) Households that are single parent (percent) by race/ethnicity 
https://data.diversitydatakids.org/dataset/11001_2_p-households-that-are-single-parent--percent--by-race-ethnicity
Calculated from American Community Survey Summary Files

5) Real Median Household Income in the United States
https://fred.stlouisfed.org/series/MEHOINUSA672N
Source of this dataset: U.S. Census Bureau  Release: Income and Poverty in the United States  
Units:  2021 CPI-U-RS Adjusted Dollars, Not Seasonally Adjusted

## Conclusion
The data analysis visualizes the significant changes in single parent percentages from 1950 to 2022, as well as top states where single parents are raising families -- which have not changed much over time.  Similar ethnicities seem to comprise the largest portion of single parent mothers; but location does impact the ranking to some degree.  Married couples have a distinct advantage over single parents regarding incomes, and single fathers over single mothers.

More analysis into quartiles and ranges of income with correlating factors is needed to better understand how and whether single parents are meeting the needs of their families in a two-income society.  By carrying forward with this analysis in the future, there will be opportunity to gain more insights and understanding as to of how single parents are faring in a today's society, and what changes might be needed to support the evolving shape of American families.