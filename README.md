# stock-analysis

## Overview and Purpose of Project

The purpose of this project was to help Steve analyze a series of stocks in the green energy space on behalf of his parents, who are looking to invest in the space. To do this, we were given a dataset outlining daily trading volumes and prices for a handful of green energy stocks for 2017 and 2018. I started the analysis by using VBA loops to run through the dataset, and output total trading volumes and yearly returns for each of the tickers. While that is a good start, refractoring the code to slightly would allow us to expand this analysis beyond those handful of stocks to the entire stock market. By tweaking a few FOR loops and creating three new arrays, I was able to produce a subroutine that was not only more robust, but able to run through the data faster. 

## Results

Looking at the ticker summaries, we can see 2017 was a pretty good year for the sector. Only 1 ticker out of 12 produced a negative return, with 4 tickers (DQ, ENPH, FSLR, and SEDG) producing a return greater than 100%. However, looking at the 2018 summary for those same stocks, it shows a very different picture. That year, the majority of stocks produced a negative return, with only RUN and ENPH staying positive that year.

It also appears that my refactored script ran through the data faster and more efficiently than my original script. For the 2017 summary, my code originally ran in .85 secs, while my refactored code managed to complete the same task [in only .17 secs](

## Summary 
