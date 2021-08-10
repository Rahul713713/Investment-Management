# Investment Management : Project Overview
![investment_management](https://github.com/Rahul713713/Investment-Management/blob/master/Investment_Management.jpg "Investment Management")
- Created multiple charts,graphs,boxplots,etc. in order to understand the data and where the company should invest in order to avoid risks.
- Worked with 3 different datasets by merging them together.
- Cleaned the data in each datset and checked for missing values so that they can be merged together.
- Performed data analysis on the different datasets keeping in mind the two constraints provided by the company.

# Problem Statement

The problem involves a company which wants to make some investments in few companies to get profits.They are mostly focused on investing in young start-ups and small or mid-size companies. The head of the company wants to understand the world wide trends in investments so that the top managers can decide where they should invest to get good profits.

The company wants to invest in areas where most of the other investors are investing.Since,it's their first investment they want to play safe and avoid huge risks.The objective of this problem is to identify the best sectors, countries, and a suitable investment type for making investments. The overall strategy is to invest where others are investing, implying that the 'best' sectors and countries are the ones 'where most investors are investing'.

# Constraints

The company has two minor conditions for investments:
1. It only wants to invest in the range of 5-15 million US dollars.
2. Also,it only wants to invest in English-speaking countries i.e. countries where English is an official language.This is because of the ease of communication with the companies it would invest in. 


# Resources Used
- Python Version: 3.6.0
- Packages: pandas, numpy, matplotlib, seaborn

# Data Cleaning
## After reading the data, I needed to clean it up so that it was usable for our data analysis. After cleaning the data and handling missing values,the following features are used to determine the type of investment to be made and the best countries for investing:

 1   country_code             
 2   funded_at                
 3   funding_round_permalink  
 4   funding_round_type       
 5   main_category            
 6   name                     
 7   permalink                
 8   raised_amount_usd        
 9  status                   
 10   sector                    

# Observations
After cleaning the data,I started with EDA. These are some of the outcomes of EDA and the important results 

![loan_status vs term](https://github.com/Rahul713713/Investment-Management/blob/master/Amount_raised_across_four_categories.png "Amount_raised_across_four_categories")
![loan_status vs term](https://github.com/Rahul713713/Investment-Management/blob/master/Top_three_countries_for_investment.png "Top_three_countries_for_investment")
![loan_status vs term](https://github.com/Rahul713713/Investment-Management/blob/master/Amount_invested.png "Amount_invested")

# Results

- The company should make a venture type investment.
- The top country in terms of the number of investments (and the total amount invested) is USA. 
- The top three countries for investemnt are USA,Great Britain and India.
- The sectors 'Others', 'Social, Finance, Analytics and Advertising' and 'Cleantech/Semiconductors' are the most heavily invested ones.

In case we don't want to consider 'Others' as a sector, 'News, Search and Messaging' is the next best sector

# Project Conclusion

The company should invest in one of these top three countries: USA,Great Britain and India. The type of investment should be venture and the major sectors for investment should be 'Others', 'Social, Finance, Analytics and Advertising' and 'Cleantech/Semiconductors'.
