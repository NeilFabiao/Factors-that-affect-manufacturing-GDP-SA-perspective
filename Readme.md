# Investigating the relationship of factors that affect the growth of the Manufacturing GDP: A South African Perspective #

## Summary/Abstract

In the year of 2020, there has been an enforceable pandemic called COVID-19 that caused a global and economic shutdown with unprecedented consequences. With Gross domestic product (GDP) "a monetary measure of the market value of all the final goods and services produced in a specific time", being an indicator of countries prosperity it is essentially important to understand what variables impact the GDP of a country such as South Africa. 

The purpose of this project is to understand the factors that affect the growth of the Manufacturing GDP, the idea in this notebook is inspired from [Factors Affecting GDP (Manufacturing, Services, Industry): An Indian Perspective Dhiraj Jain, K. Sanal Nair and Vaishali Jain](https://www.scmspune.ac.in/chapter/Chapter%203.pdf). With a focus on South African context, the dependent variable will be Manufacturing GDP and the additional variables not included in the Indian Perspective such as electricity availability, number of workers in the manufacturing sector and others. 

The methodology for selecting the best model in this project was decided between a backward and forward variable selection that was adjusted according to R-squared value. After hypothesis testing and feature engineering, the model  deemed best by having a p-value above 0.05 was the forward selection and it gave the following model :


![alt-text-1](/Project/img/umage2.png) 

The result produced in the model above indicated that the countries exportation and importation served as an indicator of how much a country is self-sufficient and offers their services to other; in the case of South Africa a positive level can be assigned to the GDP since there is a sustainability factor that attracts other investors to the country. Incentives for investments that being local or foreign also played a great role in the model, leading to understand that the levels of debt and inflation motivates spending and capital circulation, and although this may be considered good or positive for GDP in a more general perspective, may be different in an in-depth view where this amount of capital may not circulate to some individuals either lower-income families or small businesses. On the other hand electricity production or difference in imported and exported electricity, in recent years has seen a decrease in production and maybe one of the factors to be considered important going forward given that the level of innovation in certain sectors depend on "Light for productivity". 

The main limitation found on the project was the data availability, given that some of the websites would not allow the public to download data from prior years to 2000 and in consequence some of the available data had quarters with missing values. Suggestion for future students is to acquire more data to provide new insights, test different modeling selection techniques and having actual quarters for some of the years not provided by the OECL. All in all from this model makes it understandable that if there is an increase in productivity and the services necessary in the world that being technology or any other, there is an increasing probability of learning from this experience and to navigate in the event of another pandemic.

## Exploratory Analyses 

### Understading South Africa GDP over years of (1993 - 2019)

The different industries that influence the GDP of South Africa such as manufacturing, retail, and electricity gas and water had a positive trend along the years of 1993 - 2019. 

From the plots bellow there is an undersranding that the Retail industry has had greatest grow potential over the years, followed by the manufacturing sector, that despite the continuous growth it saw a rapid decrease in prices in the years of 1998 and 2008 compared to other industries and is the industry that seems to suffer the most in the times of crises. The rapid decrease in prices during the years of 1996 to 1998 and 2008 can be due to the financial crises that the world suffered during that period, and that is the reason why the second plot was created to accurately visualize the year that the rapid decrease occurred. 

![alt-text-1](/Project/img/umage3.png) 

`Since the focus of this project is to study the factors that affect the growth of the Manufacturing GDP there is a necessity to visualize the performance over time.`

![alt-text-2](/Project/img/umage4.png)

### Understanding Marco economic variables over the years (1993-2018) 

#### Inflation
Inflation since 2016 has been in decline and these can be considered incentives for capital circulation. On the other hand, the exportation and importation levels in recent years reached almost similar levels just a slight variation between the two, this allows to consider that South Africa can be a sustainable country and able provide the manufacturing services to other countries.

Lower inflaction such as the one achieved in 2004 of -1%, signifies that the country has entered temporary lower growth period and is trying to regain confidence in the economy ([Monetary Developments,2012](https://www.imf.org/external/pubs/nft/2006/soafrica/eng/pasoafr/sach12.pdf)).  

![alt-text-3](/Project/img/umage5.png) 

#### Debt , export and import of goods
External debt after 2008 has seen a surge, with the highest value being 1.1 Trillion rands in 2017. On the other hand for import of Goods, it saw increase since 2003 with a slight decline in 2008, where 1.8 Trillion Rands was the highest point. For export of Goods similar to the import it saw growth since 2003 where the highest point was 1.8 Trillion Rands, the average 1 Trillion Rands and decline in 2008 because of the financial crisis.

![alt-text-4](/Project/img/umage6.png)

#### Portfolio equity and foregin investments 

Foreign direct investments registered growth in the years of 1997, 2001, 2005 and 2008 where the highest point is 1.4 Trillion Rands and 161 Million Rands as the minimum amout. On the contrast for portfolio equity the prosperour years were 1998,1999, 2006. 2009 and 2014 where the highest was 2.1 Trillion Rands and 673 Billion Rands as loss in investments in 2008 due to the economic crisis.
The negative portfolio equity in the year of 2008 was negative that simply mean that the value of an asset fell below the outstanding balance on the loan used to purchase that asset.

![alt-text-5](/Project/img/umage7.png)
#### Pie chart of average percentage of change 
Over the years the variable that has experienced highest percentage of growth has been Equity with an average of 6%, followed by foreign investments 1% and inflation 0.14%. This can be considered accurate since in recent years foreign capital has accunted for majority of South Africa and Africas development fund.

![alt-text-6](/Project/img/umage8.png)
#### Correlation matrix
The variables with low correlation to Manufacturing GDP indicated by the matrix bellow are :

- Employees in Manufacturing
- PPI (Producer Price Index)
- Inflation
- Equity 

On the other hand the variables with highest degree are :

- Available Electricity in SA
- Export Goods
- Import Goods
- Debt
- (Exported - Imported) Electricity in SA

The variables with a positive relationship, leading to us to understand that the variation or change that happens in one of the variables has a significant impact on the other, in this case Manufacturing GDP is affected by export and import of goods as well as the amount of foreign Debt allow the country of SA to move in a positive direction. In contrast the variable `(Exported - Imported) Goods in SA` is considered to be strongly uncorelated, this signifies that when the two variables (independent and dependent) tend to move, they move in opposite direction, such that when one increases the other variable decreases.

![alt-text-8](/Project/img/umage10.png)
 ![alt-text-9](/Project/img/umage9.png)

## References

1. Github and google

2. Data sources 

The first datasets was downloaded on the 3rd of March 2020 form the link [Stats Sa time series data](http://www.statssa.gov.za/?page_id=1847), where the gdp1993 database contains quarterly values collected from 1993 to 2019, while on the available electricity database we have two dataset files elecavaliable1990 and elecavaliable2000 that were also downloaded on the Stats SA website.

For the secondary dataset, there is PPI index coming from [Stats SA time series data](http://www.statssa.gov.za/?page_id=1847) and other datasets downloaded from  OECD such as:

- [OECD Inflation](https://data.worldbank.org/indicator/FP.CPI.TOTL.ZG?end=2019&locations=ZA&name_desc=false&start=1993)
- [External debt stocks, public and publicly guaranteed](https://data.worldbank.org/indicator/DT.DOD.DPPG.CD?end=2018&locations=ZA&start=1993)
- [Exports of goods and services ](https://data.worldbank.org/indicator/NE.EXP.GNFS.CD?end=2018&locations=ZA&name_desc=false&start=1993)
- [OECD Portfolio equity](https://data.worldbank.org/indicator/BX.PEF.TOTL.CD.WD?end=2019&locations=ZA&start=1993)
- [Foreign direct investment](https://data.worldbank.org/indicator/BX.KLT.DINV.CD.WD?end=2019&locations=ZA&start=1993&view=chart)
- [OECD Employment Outlook](https://data.oecd.org/emp/employment-by-activity.htm#indicator-chart)


## Who do I talk to?

* Repo owner Neil Fabião -> @neilfabiao or neilfabiao@gmail.com

## Extra info 
This project was done using jupyter-notebook, and in the Project folder there are 3 other subsequent folders namely:

* Data - where all the data used in the project is located.
* src - or source code where the implementation is stored in jupyter-notebook or html. 
* img - where the images for the readme and the jupyter-notebook are located. 

To run any of the implementations located in src simply select a file and load on your browser. 

`Note: The values for the OECD were converted to rands using value of exchange during the week of the 10th of january 2020, which is the period near the release of the data.`

<!-- Primary Meta Tags -->
<meta name="title" content="Factors that affect manufacturing GDP SA perspective">
<meta name="description" content="A study utilizing backward and forward selection to understand if the electricity availability, number of workers and others variables influence manufacturing GDP. My first Github Project 😄! ">

<!-- Open Graph -->
<meta property="og:title" content="Factors that affect manufacturing GDP SA perspective" />
<meta property="og:url" content="https://github.com/NeilFabiao/Factors-that-affect-manufacturing-GDP-SA-perspective" />
<meta property="og:description" content="A study utilizing backward and forward selection to understand if the electricity availability, number of workers and others variables influence manufacturing GDP. My first Github Project 😄!">
<meta property="og:image" content="/Project/output/extra1design.png">
<meta property="og:type" content="article" />


<!-- Extra -->
<meta property="og:locale" content="en_GB" />
<meta property="og:locale:alternate" content="fr_FR" />
<meta property="og:locale:alternate" content="es_ES" />


