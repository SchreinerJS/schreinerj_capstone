# Shape of the American Family
<div class='tableauPlaceholder' id='viz1693185365354' style='position: relative'><noscript><a href='#'><img alt='Introduction and Overview ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Sh&#47;ShapeofAmericanFamily_1P_Introduction_Overview&#47;IntroductionandOverview&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='ShapeofAmericanFamily_1P_Introduction_Overview&#47;IntroductionandOverview' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Sh&#47;ShapeofAmericanFamily_1P_Introduction_Overview&#47;IntroductionandOverview&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1693185365354');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='1700px';vizElement.style.height='1127px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

## Tableau Story
Links:
Part I
https://public.tableau.com/app/profile/jennifer.schreiner/viz/ShapeofAmericanFamily_1P_Introduction_Overview/IntroductionandOverview

Part II
https://public.tableau.com/app/profile/jennifer.schreiner/viz/ShapeofAmericanFamily_2P_ChildrensLivingSituations/ShapeoftheAmericanFamily

Part III
https://public.tableau.com/app/profile/jennifer.schreiner/viz/ShapeofAmericanFamily_3P_Factors_Impacting_Income/ShapeoftheAmericanFamily

## Table of Contents
* [Tableau Story](#Tableau-Story)
* [Overview](#Overview)
* [Motivation](#Motivation)
* [Questions](#Questions)
* [Data Cleaning and Normalizing](#Data-Cleaning-and-Normalizing)
* [Technologies Utilized](#Technologies-Utilized)
* [Issues and Limitations](#Issues-and-Limitations)
* [Conclusion](#Conclusion)
* [What Can We Do?](#What-Can_We-Do?)
* [Where Do We Go From Here?](#Where-Do-We-Go-From-Here?)
* [Sources](#sources)

## Overview
Family is the basis of society, and the shape of the American family has changed significantly since the entry of more women and mothers into the workplace. 

This analysis of historical Census Bureau and other family and household data offers insight into the changes to American family shape and structure over time, with a focus on sole (or single) parents.

In addition, analysis of historical income trends as well as other factors will raise awareness of the challenges our sole parents may be facing in a dual-income society.

## Motivation
This project was inspired by the valiant efforts of my brother as a single dad in years past, and by the stories of sole mother co-workers and friends, as well as by the data itself. 

With better understanding of the historical trends and factors impacting sole parents, such as earning potential, location, and ethnicity, more conversations and more questions can be encouraged as to how governments, communities, families, and individuals are adapting to these changes.

## Questions
Questions that focused my analysis included:

- How has the shape and structure of the American family changed over time?

- How are children's living situations being impacted by historical trends of marital status for sole parents?

- What factors are impacting earnings for sole parents, and especially, sole mothers, such as employment and income trends, number of earners, age, location, and/or race/ethinity? 

## Data Cleaning and Normalizing
Data was drawn primarily from U.S. Census Bureau Current Population Surveys Annual Social and Economic Supplements (CPS ASEC) Tables.  Additional single parent datasets were selected from datadiversitykids.org, which were calculated from Census Bureau American Community Survey (ACS) data, as well as from web scraping and custom tables from the OECD Family Database (Organisation for Economic Co-operation and Development).

The tables were cleaned and transformed in Python and Alteryx, removing footnotes and duplicated year rows (keeping the most recently compiled data), transforming datatypes, building the tables long, and selecting timeframes which had no missing data for one or more variables. 

## Issues and Limitations
Census variables and definitions have been evolving to accommodate the changes to family structure.  There were also considerations of the need to make adjustments for inflation and current dollars.  Therefore the decision was made to utilize pre-tabulated data and datasets, which offered a variety of historical household, family, and income values calculated with the appropriate year-to-year adjustments.

With more time to become familiar with the Census API, the census wrapper for Python, and other custom tools to access their Census bureau data, it would be possible to deepen the overview of changes to family structure as well as income to expense analysis.

More survey data needs to be collected to dig into how many jobs a sole parent is working to  provide for their family with or without government assistance, with or without contributions from a second parent, to reach median income levels, as variables tend to be focused toward the total earnings of an earner. 

Additional time was needed to complete the project after recognizing that the tables were joined wide in Python rather than long, which caused some issues in Tableau, but this was a good opportunity to apply the newly learned Alteryx technology to speed up the process.

## Technologies Used
1) Excel - review, some initial alteration of tables
2) Python / Pandas - exploration, normalizing, cleaning, joining, and transforming tables
3) Alteryx - normalizing, cleaning, joining, and transforming tables and datasets
4) Web scraping - minimum wage table
5) Tableau - for analysis, dashboard and story visualization
6) PowerPoint - for project overview and introduction
7) GitHub - for version control

## Conclusion
Married couples with dual incomes or earners with incomes in the highest percentiles have significant financial advantage over single parents families with only one earner who may also be disadvantaged by age, educational attainment, location, or race/ethnicity.

More than 25% of sole mothers are not able to work full-time, one reason for which could be  the cost of daycare to earning potential for those for whom remote work is not an option.  

States choosing to raise their minimum wage to $15 in support of the Raise the Wage Act[^1] could eliminate poverty wages for sole mothers, assist them to meet cost of living if not toward median wages, and could benefit all sole parents most disadvantaged by age, race/ethnicity, educational attainment, and/or location.[^2].

More data is needed to track how many jobs or hours a sole parent not in poverty is working to meet cost of living and/or the real median.

[^1]: https://www.congress.gov/bill/117th-congress/house-bill/603
[^2]: https://github.blog/changelog/2021-09-30-footnotes-now-supported-in-markdown-fields/

## What Can We Do?
Companies supporting remote or hybrid work opportunities may assist to bridge the gap between earning potential and cost of living for disadvantaged sole parents.

Higher minimum wages, especially in those states where the minimum wage has not been raised in 10 years and where there are higher percentages of disadvantaged sole mothers, would assist more children out of poverty.

Governing authorities and employers might also consider taking the lead on closing the remaining gender gap in income.

## Where Do We Go From Here?
Top states for sole mothers have not changed significantly over time.  Further analysis would explore whether sole mothers are engendering sole mothers, and whether poverty is at the heart of the trend.

Marriage is on the decline for both parent couples and sole parents.  Further study could determine any correlation with a decline in religious belief, an increase in stranger danger, or working hours are contributing factors.

## Data Sources
To answer the above questions, the tables and datasets were pulled from the following sources for analysis:

1) Various Census Bureau Historical Households and Historical Household Income Tables
https://www.census.gov/data/tables/time-series/demo/families/families.html
https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-income-households.html

2) Various Census Bureau Family Households and Historical Family Income Tables
https://www.census.gov/data/tables/time-series/demo/families/households.html
https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-income-families.html

3) Various Datasets from DataDiversityKids.org
* diversitydatakids.org. 2021. “Households that are single parent (count) by race/ethnicity”, retrieved from https://data.diversitydatakids.org/dataset/11001_2_c-households-that-are-single-parent--count--by-race-ethnicity?_external=True on May 02 2023, calculated from American Community Survey Summary Files

* “Households that are single parent (percent) by race/ethnicity”, retrieved from https://data.diversitydatakids.org/dataset/11001_2_p-households-that-are-single-parent--percent--by-race-ethnicity?_external=True on May 02 2023, calculated from American Community Survey Summary Files

* “Single mother families with children aged 0-17 years (count) by race/ethnicity”, retrieved from https://data.diversitydatakids.org/dataset/17010_3_c-single-mother-families-with-children-aged-0-17-years--count--by-race-ethnicity?_external=True, calculated from American Community Survey Summary Files

 * “Single mother families with children aged 0-17 years (percent) by race/ethnicity”, retrieved from https://data.diversitydatakids.org/dataset/17010_3_p-single-mother-families-with-children-aged-0-17-years--percent--by-race-ethnicity?_external=True, calculated from American Community Survey Summary

 * “Poverty rate, single mother families with children aged 0-17 years (percent) by race/ethnicity”, retrieved from https://data.diversitydatakids.org/dataset/17010_4_p-poverty-rate--single-mother-families-with-children-aged-0-17-years--percent--by-race-ethni?_external=True on Jun 27 2023, calculated from American Community Survey Summary Files

* “Housing units with family households (count)”, retrieved from https://data.diversitydatakids.org/dataset/25011_1_c-housing-units-with-family-households--count-?_external=True on Jun 29 2023, calculated from American Community Survey Summary Files
git

4) Real Median Household Income in the United States
https://fred.stlouisfed.org/series/MEHOINUSA672N
Source of this dataset: U.S. Census Bureau  Release: Income and Poverty in the United States  
Units:  2021 CPI-U-RS Adjusted Dollars, Not Seasonally Adjusted

5) Mininum Wage (web scraped)
https://www.hourly.io/post/minimum-wage-by-state#:~:text=Which%20States%20Have%20a%20%2415,we%20get%20to%20mid%2D2023

6) Various Custom Datasets from the OECD Family Database (Organisation for Economic Co-operation and Development)
A unique forum where the governments of 37 democracies with market-based economies collaborate to develop policy standards to promote sustainable economic growth.
https://www.oecd.org/social/family/database.htm
