# Stock Analysis

## Overview of Project

   The purpose of this analysis is to find what stocks had a gain and which stocks had a lose throughout a specific year. This allows those looking at the data to determine which stocks they would like to invest in and allow them to make the best-informed decision with the data available to them. I took data on 12 stock symbols and then ran a macro to determine the total volume of stocks traded for that symbol in that year. As well as took the lowest closing price and the highest closing price to determine the total gain or lose percentage for that year. 

## Results

For completion of this challenge, I had to refactor code that would complete the same analysis as the code completed in the module. The refactored code used a different approach to completing the task than the code we did in the module. This refactored code used three additional arrays to hold the values of volume, high price, and low price. Each array held the values for each specific ticker symbol. It would cycle through the data checking the ticker to confirm it was still viewing the right data for that symbol. If it was the correct ticker, it would increase the volume and then check closing prices to find the lowest and highest prices. If it found that the next row was a different symbol it would increase the ticker index by 1 and then loop back through to repeat the process. This process turned out to be much more efficient than the method used in the module. The module used nested for loops and just assigning variables. Below you can see the increased speed between both the module and refactored code. 

Module 2018             | Refactored 2018
:----------------------:|:----------------------------:
![Module 2018 Stocks](https://github.com/Tyfox1206/stock-analysis/blob/main/Resources/VBA_Module_timer_2018.png)|![Refactored Code 2018](https://github.com/Tyfox1206/stock-analysis/blob/main/Resources/VBA_Challenge_2018.png)
Module 2017             | Refactored 2017
![Module 2017 stocks](https://github.com/Tyfox1206/stock-analysis/blob/main/Resources/VBA_Module_Timer_2017.png)|![Refactored Code 2017](https://github.com/Tyfox1206/stock-analysis/blob/main/Resources/VBA_Challenge_2017.png)

## Summary

When refactoring it can prove to be quite beneficial. With refactored code you improve speed, readability of the code and over all functionalities. However, there is chance that you will break the code and not be able to repair it or you may cause bugs to occur that were not present in the original code. Furthermore, you can find yourself in a situation when refactoring you may have to get into files that were not originally part of the refactor. 

In this instance the advantages of using the refactored code increased speed drastically. However, when reviewing this code, there a chance for some people that the refactored code could be harder to follow at some points as there are multiple arrays being worked through while the original code only has one array, and the rest was variable assignment. The refactored VBA script does work better, and I personally find it easier to follow compared to its variable assignment counterpart. The trouble shooting was easier since I could view the value of each array element and did not have to follow one specific variable changing throughout its run time. 
