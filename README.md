# Indeed Wage Tracker
 
**Note**: May 2023 data marks a new release of the Indeed Wage Tracker, a measure of wage growth in job postings in eight countries. Indeed Hiring Lab is committed to delivering reliable, trustworthy, and comprehensive data and analysis of the global labor market. An upgrade to our internal salary data platform and enhancements to the ways Indeed classifies job titles in certain countries over the past several months delayed our usual publication of the wage tracker. These efforts, aimed at improving the quality of the data, led to small changes in the historical wage growth series compared with previously published data, but did not impact the fundamental trends.

The Indeed Wage Tracker measures growth in wages advertised in job postings to help policymakers, labor market analysts, employers, and workers understand wage trends quickly and confidently.
 
We currently publish country-level trends for 8 countries: the UK, the US, and six euro-area countries — France, Germany, Ireland, Italy, the Netherlands, and Spain — that jointly account for over 80% of euro-area employment.
 
We will add more countries over time. We also plan to add data on wage growth in individual occupational categories, as we do in our [Job Posting Index](https://github.com/hiring-lab/job_postings_tracker).
 
The Indeed Wage Tracker will be updated monthly, with the exact timing depending upon Hiring Lab’s publication schedule.
 
## Methodology
 
The data in this repository are the average year-on-year percentage changes in wages and salaries advertised in job postings on Indeed, controlling for job titles. 
 
To calculate the average rate of wage growth, we follow an approach similar to the Atlanta Fed [US Wage Growth Tracker](https://www.atlantafed.org/chcs/wage-growth-tracker), but we are tracking job titles, not individuals. We begin by calculating the median posted wage for each country, month, job title, region and salary type (hourly, monthly or annual). Within each country, we then calculate year-on-year wage growth for each job title-region-salary type combination, generating a monthly distribution. Our monthly measure of wage growth for the country is the median of that distribution. The data are not seasonally adjusted.

More information about the data and methodology is available in our accompanying research paper, [“Wage growth in Europe: evidence from job ads”](https://www.centralbank.ie/page-not-found-404?aspxerrorpath=/docs/default-source/publications/economic-letters/wage-growth-europe-evidence-job-ads.pdf) (Adrjan and Lydon, 2022), published in the Central Bank of Ireland’s Economic Letter series. We adopted this methodology in October 2022.
 
For Frequently Asked Questions regarding Indeed's data, click [here](https://www.hiringlab.org/indeed-data-faq/).

## Data Schema
 
The CSV file contains the following variables:

- jobcountry: two-letter code of the country of the Indeed site where the job was posted
- country: country name
- month: the month when the job was first posted
- posted_wage_growth_yoy: the year-on-year change in posted wages calculated using the methodology described above
- posted_wage_growth_yoy_3moavg: the 3-month lagged moving average of posted_wage_growth_yoy, which we use as our headline measure of growth
 
## Indeed Hiring Lab
 
The [Indeed Hiring Lab](http://hiringlab.org/) is an international team of economists and data scientists dedicated to delivering insights that help drive the global labor market conversation.
 
This GitHub repo is intended to serve as a space to host various regularly-updated data series to help economists, journalists, and other interested parties better understand the labor market conditions in their countries.
 
We have economists covering Australia, Canada, France, Germany, Ireland, Japan, the UK, and the US. To read our research, visit the Indeed Hiring Lab blog: [https://www.hiringlab.org](https://www.hiringlab.org/).
