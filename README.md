# Voting Power By Demographic 

This repository contains the data and analysis for the BuzzFeed News article, "[How The Electoral College Screws Hispanic And Asian Voters](https://www.buzzfeed.com/johntemplon/how-the-electoral-college-screws-hispanic-asian-vo)," published November 7, 2016.

## Data

The data for this analysis came from two sources:

- __The U.S. Census__. The [`data/census`](data/census) contains two files: `Table 4b` from the Census's [Voting and Registration in the Election of November 2012](https://www.census.gov/hhes/www/socdemo/voting/publications/p20/2012/tables.html) and a slice of the Census's Current Population Survey, which was obtained through the [CPS Table Creator](http://www.census.gov/cps/data/cpstablecreator.html).

- __FiveThirtyEight__. This analysis uses [FiveThirtyEight's "Voter Power Index"](https://projects.fivethirtyeight.com/2016-election-forecast/#tipping-point) estimates for the 2016 election. BuzzFeed News downloaded the data on November 5, 2016; you can find it in the [`data/fivethirtyeight`](data/fivethirtyeight) directory. The code used to collect the data can be found [in this notebook](notebooks/scrape-voter-power-index.ipynb).

## Analysis

The full analysis [can be found here](notebooks/demographic-analysis.ipynb). The first part of the analysis uses the Voter Power Index and 2012 voter registration data to quantify relative voting power vis-a-vis race. The second part of the analysis examines relative voting power vis-a-vis education. That analysis uses the CPS's counts of *adult citizens*, because the Census does not produce state-level counts of registered voters by educational attainment.

## Questions / Comments?

Please contact John Templon at john.templon@buzzfeed.com.

Looking for more from BuzzFeed News? [Click here for a list of our open-sourced projects, data, and code](https://github.com/BuzzFeedNews/everything).
