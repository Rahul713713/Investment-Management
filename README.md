# Investment-Management : Project Overview

- Created multiple charts,graphs,boxplots,etc. in order to understand how to minimise the risk of losing money while lending to customers.
- Worked on a dataset consisting of 39717 rows of data for 111 different features.
- Performed univariate analysis as well as multivariate analysis on various features to understand the importance of every feature.
- Used EDA to understand how consumer attributes and loan attributes influence the tendency of default rate.Thus,helped the company in understanding the driving factors (or
driver variables) behind loan default, i.e. the variables which are strong indicators of default.

# Problem Statement

The problem involves a company which wants to make some investments in few companies to get profits.They are mostly focused on investing in young start-ups and small or mid-size companies. The head of the company wants to understand the world wide trends in investments so that the top managers can decide where they should invest to get good profits.

The company wants to invest in areas where most of the other investors are investing.Since,it's their first investment they want to play safe and avoid huge risks.The objective of this problem is to identify the best sectors, countries, and a suitable investment type for making investments. The overall strategy is to invest where others are investing, implying that the 'best' sectors and countries are the ones 'where most investors are investing'.

# Constraints

The company has two minor conditions for investments:
1. It only wants to invest in the range of 5-15 million US dollars.
2. Also,it only wants to invest in English-speaking countries i.e. countries where English is an official language.This is because of the ease of communication with the companies it would invest in. 


# Code and Resources Used
- Python Version: 3.6.0
- Packages: pandas, numpy, matplotlib, seaborn

# Data Cleaning
## After reading the data, I needed to clean it up so that it was usable for our data analysis. I made the following changes and created the following variables:
- Checked whether we have missing data for various cloumns.
- Since,many columns had 33%,65% and even 100% missing values,I deleted those columns as they played no part in deciding the defaulting customers. 
- Extracted the numeric part from the variable employment length.Also,deleted the missing values from the same column. 
- Now, there are broadly three types of variablesin our dataset - 1. those which are related to the applicant (demographic variables such as age, occupation, employment details etc.), 2. loan characteristics (amount of loan, interest rate, purpose of loan etc.) and 3. Customer behaviour variables (those which are generated after the loan is approved such as delinquent 2 years, revolving balance, next payment date etc.).I decided to drop the customer behaviour variables as they are not available at the time of loan application, and thus they cannot be used as predictors for credit approval.
- Also, we will not be able to use the variables zip code, address, state etc. The variable 'title' is derived from the variable 'purpose'.Thus,I got rid of all these variables as well
- Converted loan_status to integer type in order to get the total number of customers who defaulted and who didn't.
- Finally,the remaining columns used for EDA are

 1   id                         
 2   member_id                  
 3   loan_amnt                 
 4   funded_amnt                   
 5   funded_amnt_inv             
 6   term                        
 7   int_rate                    
 8   installment                 
 9   grade                        
 10  sub_grade                   
 11  emp_title                    
 12  emp_length                  
 13  home_ownership               
 14  annual_inc                  
 15  verification_status          
 16  issue_d                      
 17  loan_status               
 18  pymnt_plan                                            
 19  purpose                     
 20  dti                        
 21  initial_list_status          
 22  collections_12_mths_ex_med  
 23  policy_code                   
 24  acc_now_delinq              
 25  chargeoff_within_12_mths    
 26  delinq_amnt                  
 27  pub_rec_bankruptcies        
 28  tax_liens 

# EDA
After cleaning the data,I started with EDA. These are some of the outcomes of EDA 

![loan_status vs term](https://github.com/Rahul713713/Investment-Management/blob/master/Amount_raised_across_four_categories.png "Amount_raised_across_four_categories")
![loan_status vs term](https://github.com/Rahul713713/Investment-Management/blob/master/Top_three_countries_for_investment.png "Top_three_countries_for_investment")
![loan_status vs term](https://github.com/Rahul713713/Investment-Management/blob/master/Amount_invested.png "Amount_invested")


