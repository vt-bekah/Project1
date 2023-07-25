# Project1
This repository contains challenge files for Project #1 od the UT DAV Bootcamp

# Project Proposal
In this project, we'll be working as a data analyst for a prominent real estate investment firm. Our task is to conduct in-depth research and provide expert insights to a high-profile client who is looking to invest in residential properties.
Our client wants to know which cities or regions have the highest potential for a profitable real estate investment.
Here's what your project entails:
1.	Data Collection: Utilize the Real Estate Data API to extract and aggregate a year's worth of comprehensive data on residential property sales, population growth, job market statistics, and other relevant factors for specific cities or areas of interest.
     * Target cities: Austin, New York, San Francisco, Pittsburgh, Chicago, Memphis, Denver, Las Vegas (depending on where we find adequate data)
     * Residential property sales (ideally over time)
     * Population growth
     * Job market stats – unemployment, top job types
     * Property Tax / State Income Tax
     * Potentially include rental data
2.	Market Trends: Analyze the data to identify cities or regions where property prices have been steadily increasing over the past year. Uncover hidden gems with untapped potential that could yield significant returns for your client.
     * Are there any cities that stand out not included in target list?
     * Within target list:
        * Are property sales trending up or down (quantity and price)? Potentially include rental data
        * How do property tax and state income tax compare?
        * How does population growth compare?
        * How does unemployment compare?
        * What type of jobs are most common?
3.	Demographic Analysis: Dig deeper into the demographic data provided by the API to understand the local population's preferences, buying behavior, and trends. Determine how these factors could impact future property values and demand.
     * Income
        * How does income distribution compare?
     * Size of house (# of rooms or sq. footage – not sure what is available)
        * Is there a trend over time by size?
4.	Risk Assessment: Crime Analysis 
     * What are crime trends?
        * Violent crime
        * Property Crime
5.	Recommendations: Based on our thorough analysis, provide well-founded recommendations to our client on which cities or areas are the most promising for real estate investment. Back your suggestions with concrete data-driven evidence to instill confidence in your findings.  
  


# Data Sources 
**target cities are a must:** will alter city list if gap in available data  
**over time:** last 3 years? monthly?  
**bonus:** across US to pull high/low for potential other places of interest to call out for client  

0. Overall
     * **Is there an API?** Stats about all US cities - real estate, relocation info, crime, house prices, schools, races, income, photos, sex offenders, maps, education, weather, home value estimator, recent sales, etc. https://www.city-data.com/ 
1. Real Estate (property sales - qty & $)
     * **API** Property Data API: https://www.attomdata.com/solutions/property-data-api/  
     * **API** Census Economic Indicators: https://www.census.gov/data/developers/data-sets/economic-indicators.html  
     * **API** Housing Prices: https://blog.data.nasdaq.com/api-for-housing-data  
     * **API** Realtor API: http://realtor.com/
2. Population (growth over time; specific economics?)
     * **API** Census Population Estimates and Projections: https://www.census.gov/data/developers/data-sets/popest-popproj.html  
     * **API** Census Migration Flows: https://www.census.gov/data/developers/data-sets/acs-migration-flows.html
     * **API** FRED: https://pypi.org/project/fredapi/       
3. Job Market (unemployment, top job types, bonus: job openings?)
     * **API** Census Economic Indicators: https://www.census.gov/data/developers/data-sets/economic-indicators.html  
     * ...  
4. Tax Rates (Property, Income?, Sales?)  
     * ~~Avg 2023 State Property Taxes varies by source: https://www.rocketmortgage.com/learn/property-taxes-by-state, https://belonghome.com/blog/property-taxes-by-state, https://wallethub.com/edu/states-with-the-highest-and-lowest-property-taxes/11585, https://www.bankrate.com/real-estate/property-tax-by-state/#what-are~~
     * **data** GitHub link for Tax Foundation data: https://github.com/TaxFoundation
       * **data** 2023 State Tax Collections per Capita: https://taxfoundation.org/2023-state-tax-data/
       * **data** 2023 Combined State + Local sales tax rates by state: https://taxfoundation.org/publications/state-and-local-sales-tax-rates/  
       * **data** Property tax trend by state 2020-23: https://taxfoundation.org/ranking-property-taxes-2023/
       * **data** 2023 Income tax rates by state: https://taxfoundation.org/state-income-tax-rates-2023/  
     * **API** (free trial option) Nationwide Proprty Tax Reporting: https://dna.firstam.com/taxsource 
5. Crime Rates (Violent vs. Property)
     * **API** Worldwide: https://www.crimeometer.com/crime-data-api 
     * **data** Austin: https://data.austintexas.gov/Public-Safety/Crime-Reports/fdj4-gpfu 
     * **data** San Francisco: https://datasf.org/opendata/
     * **data** Denver: https://www.denvergov.org/opendata
     * **data** Pittsburgh: https://pittsburghpa.gov/open-data/stories.html
     * **data** Las Vegas: https://files.lasvegasnevada.gov/open-data/Open_Data_Guide_for_CLV__ODSC_Approved_.pdf  
     * **data** Memphis: https://data.memphistn.gov/browse?limitTo=datasets  
     * **data** New York: https://data.cityofnewyork.us/Public-Safety/NYC-crime/qb7u-rbmr
     * **data** Chicago: https://data.cityofchicago.org/Public-Safety/Crimes-2022/9hwr-2zxp/data  
     * ...
6. Potentially add school district ratings
     * **API** Realtor API: https://www.realtor.com/
     * **API** School District API: https://www.greatschools.org/
7. Other potential
     * Areas with populations of 65,000+. Covers a broad range of topics about social, economic, demographic, and housing characteristics of the U.S. population. https://www.census.gov/data/developers/data-sets/acs-1year.html  
     * High-level detailed tables tabulated on the 1-year microdata for geographies with populations of 20,000 or more. https://www.census.gov/data/developers/data-sets/ACS-supplemental-data.html 
     * ChatGPT suggesting realtor:
        * Zillow API: Zillow, a popular online real estate marketplace, offers APIs that provide access to property data, home values, rental information, and more.
        * Realtor API: Realtor.com's API provides access to real estate listings, property details, photos, and local market trends.
        * Redfin API: Redfin's API offers access to real estate listings, property details, and local market information, including home sale data and pricing trends.
        * Trulia API: Trulia, another prominent online real estate platform, provides APIs that offer access to property data, neighborhood details, and local market trends.
        * MLS (Multiple Listing Service) API: MLS APIs are offered by various local real estate boards and associations, providing access to real-time property listings, sales data, and more.
        * Estated API: Estated provides APIs for property data, including property details, ownership information, and historical sales data.
        * Walk Score API: Walk Score offers an API that provides walkability scores and neighborhood information to assess the accessibility and convenience of different locations.
        * Attom Data Solutions API: Attom Data Solutions provides APIs that offer access to a wide range of real estate data, including property details, ownership information, mortgage data, and more.
        * RentRange API: RentRange's API focuses on rental market data, including rental rates, vacancy rates, and rental market trends.
        * Onboard Informatics API: Onboard Informatics provides APIs that offer access to various real estate data, including property details, neighborhood demographics, and local amenities       
     * Report on Taxes across US (not per city): chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://www.lincolninst.edu/sites/default/files/pubfiles/50-state-property-tax-comparison-for-2016-full.pdf               
