# COVID-19 Software Engineer Salary Estimator Web Application: Project Overview
* Developed a web application for software engineers to get a general idea of how much they can potentially make in the United States with their level of knowledge 
* Scraped over 1000 job descriptions from glassdoor using python and selenium
* Engineered features in the application to allow customization by the user to select options that reflect their value and experience for more personalized results.

### Link: https://share.streamlit.io/mariorashadhub/covid19_software_salary_app/app.py

![alt text](https://github.com/MarioRashadHUB/covid19_software_salary_app/blob/master/images/full_app.png "Web Application")

## Code and Resources Used 
**Python Version:** 3.7

**Packages:** pandas, matplotlib, seaborn, selenium

**Ken Jee's Data Science Project from Scratch Series:**  https://www.youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t

**Data Professor's Streamlit Tutorial Series:**  https://www.youtube.com/watch?v=8M20LyCZDOY&t=300s



**Scraper Github:** https://github.com/arapfaik/scraping-glassdoor-selenium

**Scraper Article:** https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905

## Data
Tweaked the web scraper github repo (above) to scrape 1000 job postings from glassdoor.com. With each job, I got the following:
*	Job title
*	Salary Estimate
*	Job Description
*	Rating
*	Company 
*	Location
*	Company Headquarters 
*	Company Size
*	Company Founded Date
*	Type of Ownership 
*	Industry
*	Sector
*	Revenue
*	Competitors 

## Data Cleaning
The following changes were made and created the following variables before I could preform my analysis:

*	Parsed numeric data out of salary 
*	Made columns for employer provided salary and hourly wages 
*	Removed rows without salary 
*	Parsed rating out of company text 
*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 
*	Made columns for if different skills were listed in the job description:
    * Excel  
    * Powerpoint  
    * Microsoft Office  
    * Analytics  
    * Photoshop
    * Adobe
    * Adwords
*	Column for simplified job title
*	Column for description length  

## Exploratory Data Analysis
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables. 



## Model Building
Algorithmically built and tested several different models. Ridge Regression provided best results of MAE ≈ 19014.24

![alt text](https://github.com/MarioRashadHUB/covid19_software_salary_app/blob/master/images/results.png "Map of most affect states")

![alt text](https://github.com/MarioRashadHUB/covid19_software_salary_app/blob/master/images/bottom_app.png "Results from application")
