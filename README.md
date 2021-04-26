# stock-analysis

## Overview and Purpose of Project

The purpose of this project was to help Steve analyze a series of stocks in the green energy space on behalf of his parents, who are looking to invest in the space. To do this, we were given a dataset outlining daily trading volumes and prices for a handful of green energy stocks for 2017 and 2018. I started the analysis by using VBA loops to run through the dataset, and output total trading volumes and yearly returns for each of the tickers. While that is a good start, refractoring the code to slightly would allow us to expand this analysis beyond those handful of stocks to the entire stock market. By tweaking a few FOR loops and creating three new arrays, I was able to produce a subroutine that was not only more robust, but able to run through the data faster. 

## Results

Looking at the ticker summaries, we can see 2017 was a pretty good year for the sector. Only 1 ticker out of 12 produced a negative return, with 4 tickers (DQ, ENPH, FSLR, and SEDG) producing a return greater than 100%. However, looking at the 2018 summary for those same stocks, it shows a very different picture. That year, the majority of stocks produced a negative return, with only RUN and ENPH staying positive that year.

It also appears that my refactored script ran through the data faster and more efficiently than my original script. The original script was performing multiple loop iterations over the data in order to produce the summary tables, usually finishing the task in ~.85 secs. Looking at the timers for the [2017](https://github.com/matthewprice-github/stock-analysis/blob/main/VBA_Challenge_2017.PNG) and [2018](https://github.com/matthewprice-github/stock-analysis/blob/main/VBA_Challenge_2018.PNG) summaries, the refactored code performs the same task in less than half the time. While both perform the task in less than a second, if we wanted to drastically expand the data to accomodate more tickers, the speed difference between the two will increase in significance.  

## Summary 

*What are the advantages or disadvantages of refactoring code?* 
Refactoring code always has the goal of improving its efficacy and/or functionality. This can mean simplyfying processes within the code, replacing "magic numbers" and specific inputs with robust variables, or reorganizing the code to improve readability. Refactoring code can allow scripts/programs to execute faster, run with fewer errors and bugs, as well as increase in scale. 

However, refactoring code does not actually change the original function/process of the code, and requires time/resources diverted to code that technically already works. Also, simplifying complex code down to it's most efficient/essential form could in some cases lead to issues, especially if there are a lot of caveats with a particular task or dataset. 

*How do these pros and cons apply to refactoring the original VBA script?*
In our case, refactoring the code certainly improved the speed of the task, as it only used one FOR loop that chruned through the stock data, instead of two nested loops in the original script. Adding the arrays into the refactored code also makes it easier to expand the scale of tickers analyzed, which Steve seems interested in doing.

However, while this does simplify the process, the refactored code would only work if the data sets were perfectly sorted. If the rows of data were not already sorted by ticker, then the refactored code would not have worked, while the original script would have! So in that specific hypothetical, the original script is actually more robust than the refactored script. 
